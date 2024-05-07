# ABM-Project

# Transcriptome Reconstruction with Machine Learning Models

## Abstract

The premise of the paper [1] we chose is to utilize machine learning models to rebuild a transcriptome when presented with a subset of genes. This type of problem is primarily data processing related to bioinformatics and computational biology. Predicting the whole transcriptome could have significant implications in biological and clinical applications. A transcriptome put simply is the total set of RNA molecules, including messenger RNA (mRNA), present in a cell at a specific time under specific conditions. Through profiling the transcriptome it is possible to uncover disease mechanisms, propose novel drug targets, propose a basis for comparative genomics, etc. Similarly acquiring a holistic understanding of the transcriptome allows researchers to gain insights into cellular processes, developmental stages, and responses to environmental stimuli. Genomics itself is a complex topic. Specifically, by reconstructing the transcriptome from a subset of genes using machine learning models, the authors aim to address the difficulty of incomplete or sparse gene expression data, which is common in many experimental settings. This approach has the potential to enhance our ability to analyze and interpret gene expression data, leading to more accurate predictions of gene functions, regulatory networks, and disease pathways.

## Steps to Execute Code

1. **Download Data**:
   - Store respective data within your drive at the following directory path:
     ```
     '/content/drive/My Drive/MCS/SPRING2024/CS598_Final'
     ```
   - GTEX CSV: [Download Here](https://uofi.box.com/v/gtexProcessed)
     - Processed GTEX CSV data must be stored at file config DPATH + '/Gene_Read_Counts_GTEx_Adrenal_Gland.csv'
   - GTEX RAW: [Download Here](https://uofi.box.com/v/gtex-RawData)
     - Raw GTEX data must be stored at file config DPATH + '/Gene_Read_Counts_GTEx_Adrenal_Gland.gct'
   - DATA Image: [Download Here](https://uofi.box.com/v/gtex-Dataset)
   - YAML Model Config: [Download Here](https://uofi.box.com/v/yaml-ModelConfig)
     - YAML model config specifications must be stored at file config DPATH + '/default_GTEx_inplace_GAINGTEx.yaml'
   - METADATA: [Download Here](https://uofi.box.com/v/gtexMetadata)
     - Metadata config specifications must be stored at file config DPATH + '/GTEx_Analysis_v8_Annotations_SubjectPhenotypesDS.txt'
   - METADATA Image: [Download Here](https://uofi.box.com/v/gtexMetadataSnap)

2. **Obtain an API key for wandb**:
   - Wandb is imperative to running the code. An account and an API Key can be created/received at: [Wandb Homepage](https://wandb.ai/home)

3. **Create a results folder**:
   - Create a results folder within the same level as the rest of the data, so that when the model completes training it can input statistics there.

4. **Execute Code and Modify Parameters**:
   - Execute the code and modify parameter values as fit.
