
# Genomic_and_Epigenetics_of_the_Brain

Course Project completed Fall 2021 at Carnegie Mellon University \| Teammate: Justin Hoffman

This project aims to 1) identify epigenetic regions that associate with evolution of different social group sizes in primates; 2) investigate its implications in schizophrenia. Predicted open chromatin level of each region that are present in the ATAC-seq data is kindly provided by Dr. Andreas Pfenning. Please read Final Report.docx for details of the project and conclusions 

- Files with names starting with ATACSeqAnalysis are the source code written to address the first objective in six chosen primate species.   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Note: ATACSeqAnalysis_ConvertToBED is in Python, while the others are in R.       
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ATACSeqAnalysis_MSND1.ipynb and ATACSeqAnalysis_MSND2.ipynb identify the locations of 400 predicted open chromatin regions that are most positively or negatively correlated with social group size in MSN D1 neurons and MSND2 neurons.      
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ATACSeqAnalysis_ConvertToBED.py converts the results to BED.

- PhylogeneticTree.ipynb generates the phylogenetic tree of the six primate species, pruned from the Zoonomia tree.

- The txt files are genes associated with (likely regulated by) the 400 predicted open chromatin regions. This is generated by GREAT. They are called by SchizophreniaRNAseqAnalysis_Normalization&Ttest.ipynb and SchizophreniaRNAseqAnalysis_MachineLearning.ipynb.

- Files with names starting with SchizophreniaRNAseqAnalysis are written to address the second objective. They are written in Python.     &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SchizophreniaRNAseqAnalysis_Normalization&Ttest.ipynb tests if the top four genes associated with social group size are differentially expressed in schizophrenic vs non-schizophrenic prefrontal cortex samples.    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;SchizophreniaRNAseqAnalysis_MachineLearning.ipynb investigates whether the gene expression profile of the genes associated with the 400 predicted open chromatin regions can be used to predict schizophrenic and non-schizophrenic phenotype.
