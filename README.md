# 3Mcor
R-Metabolome-Microbiome-Meta Data Correlation Analysis

Dandan Liang and Tianlu Chen*
Contact: chentianlu@sjtu.edu.cn

1、Introduction
The Metabolite-Microbiome (16s rRNA)-Meta data correlation analysis method (3Mcor) is an cross-omics data analysis method based on WGCNA (weighted gene co-expression network analysis). It is designed for the correlation analysis among metabolites, microbial 16s rRNA and phenotypes, and for phenotype-relevant biomarkers screening. The main steps of 3Mcor include the dimension reduction of metabolome and microbiome data to dozens of modules, the identification of key modules which are highly correlated to each other and to the phenotype, and the identification of key metabolites or microbes within the key modules. Some strengths of 3Mcor are as follows. (1) The ideas of co-expression, co-regulation or interaction of related genes were incorporated and hence both data characteristics and biological links (pathways and inter-associations) were considered for module construction. (2) The top-down analysis strategy is effective to find out key biomarkers quickly. (3) The 3D linkages of phenotype, microbiome and metabolome contain more information and are conducive to a better understanding of biological and medical phenomena. (4) R code and demo data are available for academic use.

2、Steps for usage
1)	Install R，R Studio；
2)	Install the required R package：
install.package (WGCNA) ### -	Clustering software. Previously reported work done ###using v1.34
install.package (flashClust) ### Clustering software
install.package (ppcor) ### Partial Spearman correlations, for confounder analysis. ###previously reported work done using v1.0
install.package (gplots) ### Plotting
install.package (cowplot) ### Plotting; to arrange several plots on the same page
install.package (ggplot2) ### Plotting
install.package (plyr) ### Data transformations
3)	Operation procedure：
Firstly, store the input data in the specified location. Then, double-click to open the protocol.Rproj file. And then run the code of protocol_all.R. Finally, read the results in the specified output data path.
Note：
Input data is stored by default at D:\3Mcor-protocol\top\data
The output data is stored by default at D:\3Mcor-protocol\top\result

For more information, please see the manual.pdf
