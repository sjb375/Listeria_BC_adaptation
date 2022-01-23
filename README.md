# Listeria_BC_adaptation

The following study was funded by the Center for Produce Safety (2020CPS11)

Note: This repository contains codes and datasets for conducting statistical analysis and making figures & tables.

ABSTRACT:
Presence of and selection for Listeria spp. and Listeria monocytogenes that are less effectively inactivated by quaternary ammonium compounds (such as benzalkonium chloride [BC]) is a food safety concern, including in fresh produce environments. An initial MIC assay on 67 produce-associated Listeria strains showed that strains carrying BC resistance genes bcrABC (n=10) and qacH (n=1) showed higher MIC (4-6 mg/L BC) compared to strains lacking these genes (MIC of 1-2 mg/L BC). Serial passaging experiments that exposed the 67 strains to increasing BC concentrations revealed that 62/67 strains showed growth in BC concentrations above their parent MIC (range of 4-20 mg/L). Two serially passaged isolates were obtained for each parent strain and substreaked onto BHI agar in the absence of BC for seven rounds; 105/134 substreaked isolates showed higher substreaked MIC (range of 4 – 6 mg/L) compared to parent MIC. These results suggested isolates acquired genetic adaptations that confer BC resistance. Substreaked isolates were characterized by a combination of whole genome sequencing and Sanger sequencing of fepR, a local repressor of the MATE family efflux pump FepA. These data identified nonsynonymous fepR mutations in 48/67 isolates including 24 missense, 16 nonsense, and 8 frameshift mutations. The mean inactivation of substreaked isolates after exposure to use level concentrations of BC (300 mg/L) was 4.48 log, which was not significantly different from inactivation observed in parent strains. Serial passage experiments performed on cocultures of Listeria strains containing bcrABC or qacH did not yield growth at higher BC concentrations than monoculture experiments. 

DESCRIPTION OF FILES

The following data sets were used for data analysis for the CPS Sanitizer project:

"MIC_data.csv" - Minimum inhibitory concentration data for three different MIC assays (parent MIC, serial passaged MIC, and substreaked MIC) to benzylkonium chloride, and Listeria isolate metadata

"FoldChange_data.csv" - Fold change data for the fold changes observed for each Listeria isolate's MIC value from three different MIC assays (parent MIC, serial passaged MIC, and substreaked MIC) 

"fepR_SNP_analysis.csv" - Data describing mutations in gene encoding transcriptional regulator FepR for individual Listeria isolates, as well as substreaked MIC values for each Listeria isolate

"UseLevel_data.csv" - Microbial count data and associated Listeria isolate metadata for assay assessing of Listeria isolates to use level concentration of benzalkonium chloride

"CoCultureSummary_data.csv" - Minimum inhibitory concentration data for monocultures and cocultures of L. monocytogenes to benzalkonium chloride, and Listeria isolate metadata

The following Rmarkdown files were used to perform data analysis for the CPS Sanitizer project:

"MIC_data.analysis.Rmd" - Building linear mixed effects models analyzing Listeria MIC data using  "MIC_data.csv", "FoldChange_data.csv", "fepR_SNP_analysis.csv", and CocultureSummary_data.csv" data sets

"UseLevel_data.analysis.Rmd" - (i) Performing unpaired t-test comparing parent and adapted Listeria isolates for their response to exposure to use level concentrations of benzalkonium chloride, (ii) building a linear model analzying the effect of presence of a benzalkonium chloride resistance gene in parent strains on the response of log reduction upon exposure to use level concentrations of benzalkonium chloride, and (iii) making figures associated with the use level experiments.
