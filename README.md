# Novel Reporter Constructs to Accelerate Antiviral and Therapeutic Discovery for Enterovirus-A71
https://doi.org/10.1016/j.antiviral.2025.106094

## *Abstract*

Enterovirus A71 (EV-A71) is an important human pathogen and ‘prototype pathogen’ for studies of other Enteroviruses of pandemic potential. Understanding the biology of EV-A71 would inform generalizable strategies for antiviral drug, vaccine, and monoclonal antibody development. Such studies are accelerated by robust reagents to evaluate efficacy. Here, we describe and evaluate a suite of synthetic reporter constructs to accelerate EV-A71 research and therapeutic discovery. These constructs include replicons and infectious clones carrying luminescent and fluorescent reporter proteins. Among the reporters we tested were shorter luminescent and de novo-designed synthetic fluorescent proteins, which enhance genetic stability, reduce reporter gene loss and improve the utility of these reporters. This toolbox provides free access to robust and flexible assays for EV-A71 infection and replication through public repositories, promoting and accelerating open scientific discovery for this understudied emerging pathogen. 

-----

<https://github.com/QVEU/EVA71_Reporters>

This data repository is related to "Novel Reporter Constructs to Accelerate Antiviral and Therapeutic Discovery for Enterovirus-A71 ", William Bakhache, Ann Shen, Walker Symonds-Orr, Megan Culler Freeman, Patrick T. Dolan. Antiviral Research (2025). [https://doi.org/10.1016/j.antiviral.2025.106094](https://doi.org/10.1016/j.antiviral.2025.106094) This data repository contains code for figure generation and analysis, Neo2 and CellProfiler protocols, and sequences of plasmids.

Description of the data and file structure are below.

Correspondence can be sent to Patrick.Dolan@nih.gov
Quantitative Virology and Evolution Unit, NIH-NIAID: https://qveu.github.io/QVEU/

## Description of the data and file structure

### 1. Plasmids
Contains all the molecular biology supplementary information regarding the reporter viruses and molecular clones. The plasmids include molecular clones and replicons for the EV-A71 (strain Tainan/4643/98, Genbank accession: AF304458.1) that encode different reporter genes. 

For the folder "Viral_Molecular_Clone", there is a total of eight plasmids:

puc19-ev71-twtainan1998_4643_BB_free: EV-A71 molecular clone that is domesticated from BsAI and BsmBI sites for rapid golden gate cloning.
Molecular_Clone_001_EVA71_Insertional_handle_Position_1_2A and Molecular_Clone_002_EVA71_Insertional_handle_Position2_2A: Same as the above clone but with an insertional handle either at position 1 or 2 at the N-terminus of 2A. Insertional handle allows for rapid exchange of inserts using BsAI golden gate cloning
Molecular_Clone_003_EVA71_mBaoJin_Position_1_2A: EV-A71 molecular clone with the reporter gene mBaoJin at position 1 in 2A
Molecular_Clone_004_EVA71_mNeonGreen_Position_2_2A: EV-A71 molecular clone with the reporter gene mNeonGreen at position 2 in 2A
Molecular_Clone_005_EVA71_mRuby3_Position_1_2A: EV-A71 molecular clone with the reporter gene mRuby3 at position 1 in 2A
Molecular_Clone_006_EVA71_Nanoluc_Position_1_2A: EV-A71 molecular clone with the reporter gene Nanoluc at position 1 in 2A
Molecular_Clone_007_EVA71_mFAP10_Position_1_2A: EV-A71 molecular clone with the reporter gene mFAP10 at position 1 in 2A

The folder "Viral_Molecular_Clone/BsaI_Inserts" contains all the inserted sequences for the reporter genes flanked with BsaI sites.

The folder "GoldenGate_Assembly_Strategy_Molecular_Clone" contains the inverse PCR primers and the sequences for inserting the insertional handle at the N-terminus of 2A.

For the folder "Replicon", there is a total of five plasmids:

Replicon001_EVA71_Insertional_handle: The EVA-71 replicon consists of the 5’UTR of the virus, a start codon followed directly by an insertional handle, 30 base pairs of the C-terminus of VP1, and the complete replication proteins with the 3’UTR. Insertional handle allows for rapid exchange of inserts using BsAI golden gate cloning
Replicon002_EVA71_mBaoJin: The EV-A71 replicon with the mBaoJin reporter gene
Replicon003_EVA71_mNeonGreen: The EV-A71 replicon with the mNeonGreen reporter gene
Replicon004_EVA71_mRuby3: The EV-A71 replicon with the mRuby3 reporter gene
Replicon005_EVA71_NanoLuc: The EV-A71 replicon with the NanoLuc reporter gene

The folder "Replicon/HiFi_Assembly_Strategy_Replicon" contains the strategy for assembly of the replicon.

The folder "Replicon/BsaI_Inserts" contains all the sequences for the inserted reporter genes flanked with BsaI sites.

For the folder "NLS_BFP_Lentivirus_Plasmid", there is one lentiviral plasmid sequence: This modified version produced by Marvin Tanenbaum's lab contains a lentiviral transfer plasmid pHR_SFFV allowing expression of the blue fluorescent protein fused with a nuclear localization signal.

### 2. R_Code_Figure_Generation
This folder contains the R code along with the data frames required for generation of figures in the paper.

### 3. Imaging_Data_and_Analysis (Note: Not deposited here, due to size)
This folder contains original images, CellProfiler analysis, and R code for figure generation.

The folder "Imaging_Data_and_Analysis/Fixed_Imaging" contains all images of fluorescent viruses as well as the CellProfiler analysis of the images with the R code used to visualize the CellProfiler data. 

The folder "Imaging_Data_and_Analysis/Live_Imaging" contains a time series of cells infected with mNeonGreen-2A virus.

The folder "Imaging_Data_and_Analysis/Spinal_Organoids_MFAP10" contains images of human spinal organoids infected with mFAP10. Wells A1-A6 are non infected organoids. Wells A7-A9 are infected organoids with MFAP10. A10-A12 are infected organoids treated with 1 uM of Rupintrivir.

### 4. BioTek_Synergy_Neo2_Protocols
Contains the Neo2 protocols to run the fluorescence (Fluorescence_kinetics_protocol.prt) and luminescene (Luminescence_kinetics_protocol.prt) readings on the BioTek Gen5/3.12 software. 

### 5. Tapestation_Data
Original and complete images of the tapestation data for amplicons shown in the paper.

## 6. Structural_Analysis
All the Chai Discovery structure prediction outputs for 2A fusion proteins with the reporter genes.

## Sharing/Access information
Deposition is currently being reviewed by [BEI Resources](https://www.beiresources.org/About/BEIResources.aspx). Accession will be updated here when approved. 

## Code/Software
Data analysis and visualization was performed with R (version 4.3.3) using the tidyverse, ggplot2 and lubridate packages. Imaging data processing was performed using Fiji/ImageJ  (version 2.14.0) and CellProfiler (version 4.2.6). Molecular graphics and analysis was performed using UCSF Chimera X (version 1.8).
