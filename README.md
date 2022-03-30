# Camelina-sativa-gene-expression-analysis
Gene expression analysis of Camelina transgenics expressing LIP36 gene

Dataset and analysis focus
Gene expression dataset (GEdata) was utilized in the current study
- The dataset includes gene expression data (in TPMs) of Camelina seeds expressing LIP36 gene (mutant) and WT seeds (control).
- The expression of a total of 178836 genes in the two genotypes (WT and LIP36) was analyzed.
- The dataset columns are gene IDs, gene expression data from three biological replicates of each genotype (WT-14 B1-B3, and LIP36-14 B1-B3).

The analysis using jupyter notebook focuses on:
1) Data wrangling
2) Data filtering
3) Exploratory data analysis
4) Differential expression analysis 5) Correlation analysis

Data Preparation and Cleaning
Our workflow reported in the current analysis includes:
1) Data wrangling
2) Data filtering
3) Exploratory data analysis
4) Differential expression analysis 5) Correlation analysis
- The original dataset (GEdata) contains gene expression data (in TPM) were cleaned to remove genome duplicates (gene IDs ended with ‘_2’); were transformed to log2 for statistical analysis.
- The original dataframe (contains both WT and LIP36 expression data) was splitted into two dataframes (one for WT and one for LIP36) to facilitate comparative analyses. dropped.filter function and RegExp were used to split the dataframe. Also, rows with 0 values were dropped.
- Data filtering was applied to report the up-regulated genes (fold change, log2-FC > 2) and down-regulated genes (log2-FC < -2) from the list of DEGs

Research Question(s)
This research was designed to investigate the changes in gene expression in Camelina mutant (LIP36) to interpret the associated changes in metabolic profiling and seed yield attributed phenotypes.
In the current final project, I did utilize Data Science tools and resources to specifically answer these two questions
1) How Camelina transcriptome (RNA-seq) has changed in response to LIP36 gene expression in the LIP36 mutant relative to its WT control?
2) What are the top differentially regulated genes(DEGs, up or down) which could be good candidates for further investigations?
3) How the DEGs are correlated in terms of patterns of gene expression?

The datasets utilized in the current final project was an output of the research project funded by the Department of Energy - Biosystems Design to Enable Next- Generation Biofuels and Bioproducts (Award #DE-SC0018269).
The jupyter notebook was modified/forked from the following workflows: 
- https://github.com/francismjenkins/Capstone_project
- https://github.com/LivLilli/Differentially-Expressed-Genes-Analysis
I also acknowledge the available online resources for problem solving with python coding and analysis workflows, and anyone I obtained help from throughout this research.
