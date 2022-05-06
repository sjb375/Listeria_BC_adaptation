# Listeria_BC_adaptation

The following study was funded by the Center for Produce Safety (2020CPS11)

Note: This repository contains codes and datasets for conducting statistical analysis and making figures & tables.

ABSTRACT:
Selection for Listeria monocytogenes strains that are tolerant to quaternary ammonium compounds (such as benzalkonium chloride [BC]) is a concern across the food industry, including in fresh produce processing environments. This study evaluated the ability of 67 strains of produce-associated L. monocytogenes and other Listeria spp. (“parent strains”) to show enhanced BC tolerance after serial passaging in increasing BC concentrations and to maintain this tolerance after substreaking in the absence of BC. After serial passaging in BC, 62/67 “BC passaged cultures” showed higher MICs (4 to 20 mg/L) than parent strains (2 to 6 mg/L). After the substreaking of two isolates from BC passaged cultures for each parent strain, 105/134 “adapted isolates” maintained MICs (4 to 6 mg/L) higher than parent strain MICs. These results suggested that adapted isolates acquired heritable adaptations that confer BC tolerance. Whole-genome sequencing and Sanger sequencing of fepR, a local repressor of the MATE family efflux pump FepA, identified nonsynonymous fepR mutations in 48/67 adapted isolates. The mean inactivation of adapted isolates after exposure to use-level concentrations of BC (300 mg/L) was 4.48 log, which was not significantly different from inactivation observed in parent strains. Serial passaging of cocultures of L. monocytogenes strains containing bcrABC or qacH did not yield adapted isolates that showed enhanced BC tolerance in comparison to that of monocultures. These results suggest that horizontal gene transfer either did not occur or did not yield isolates with enhanced BC tolerance. Overall, this study provides new insights into selection of BC tolerance among L. monocytogenes and other Listeria spp.

DESCRIPTION OF FILES

The following data sets were used for data analysis for the CPS Sanitizer project:

"MIC_data.csv" - Minimum inhibitory concentration data for three different MIC assays (parent MIC, BC passaged MIC, and adapted MIC) to benzalkonium chloride, and Listeria isolate metadata

"FoldChange_data.csv" - Fold change data for the fold changes observed for each Listeria isolate's MIC value from three different MIC assays (parent MIC, BC passaged MIC, and adapted MIC) 

"fepR_SNP_analysis.csv" - Data describing mutations in gene encoding transcriptional regulator FepR for individual Listeria isolates, as well as adapted MIC values for each Listeria isolate

"UseLevel_data.csv" - Microbial count data and associated Listeria isolate metadata for assay assessing of Listeria isolates to use level concentration of benzalkonium chloride

"CoCultureSummary_data.csv" - Minimum inhibitory concentration data for monocultures and cocultures of L. monocytogenes to benzalkonium chloride, and Listeria isolate metadata

The following Rmarkdown files were used to perform data analysis for the CPS Sanitizer project:

"MIC_data.analysis.Rmd" - Building linear mixed effects models analyzing Listeria MIC data using  "MIC_data.csv", "FoldChange_data.csv", "fepR_SNP_analysis.csv", and CocultureSummary_data.csv" data sets

"UseLevel_data.analysis.Rmd" - (i) Performing unpaired t-test comparing parent and adapted Listeria isolates for their response to exposure to use level concentrations of benzalkonium chloride, (ii) building a linear model analyzing the effect of presence of a benzalkonium chloride resistance gene in parent strains on the response of log reduction upon exposure to use level concentrations of benzalkonium chloride, and (iii) making figures associated with the use level experiments.
