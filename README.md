# Code for: Increasing absolute prey density within a mimicry complex protects aposematic models and their Batesian mimics 

**Corresponding Author:** Abigail E. Robinson 

**Abstract:** Batesian mimicry is a defensive adaptation where predators learn to avoid aposematic prey and generalize their warning signals to phenotypically similar mimics. The phenotypic accuracy needed for mimics to benefit from this adaptation depends on the relative densities of models and mimics and the model’s unpalatability. As aposematic models become more unpalatable or more common relative to their mimics, warning signals become stronger, allowing even poor mimics to benefit. However, few studies have disentangled the importance of relative frequencies of models and mimics from absolute density of the prey community (both models and mimics) in driving relaxed selection on mimicry. Here, we test the hypothesis that increasing model unpalatability and absolute prey community density accelerates predator avoidance learning and enhances protection for mimics. Using replicas of the model Adelpha iphiclus (Linnaeus, 1758), its mimic Adelpha serpa (Boisduval, 1836), and the palatable control Junonia evarete (Cramer, 1779), we conducted field experiments that enhanced model unpalatability and doubled absolute prey density while maintaining a constant ratio of model, mimic, and control phenotypes. We found that enhanced model unpalatability and increased absolute density significantly reduced predation on all species, highlighting absolute community density as an underappreciated mechanism shaping selection on Batesian mimics.

**Description of data files:** This data upload includes all code and data files for the paper entitled "Increasing absolute prey density within a mimicry complex protects aposematic models and their Batesian mimics". Details for all unique variables are described below 

- **"absolute_density_analysis.Rmd":** This R Markdown file contains the code for generating maps, fitting GLMMs and Cox Proportional Hazards models to data from the file named "density_data_binomial.csv", including data cleaning, model selection, and visualization of results. 

Within the **data_files** folder:

- **"density_data_binomial.csv":** This CSV file contains the raw data collected from the field experiments, including information on predation events, species identity, treatment groups, and other relevant variables. For the unpalatability_treatment variable, "no" indicates that model unpalatability was not experimentally enhanced with a 2% Bitrex solution, while "yes" indicates that model unpalatability was enhanced with the Bitrex solution. For the density_treatment variable, "low" indicates that a given field site was under low asbolute prey density conditions (i.e., 20 facsimilies / species), while "high" indicates that a given field site was under high absolute prey density conditions (i.e., 40 facsimilies / species). Experimental_day indicates the day (1-4) on which attack data was collected. Site indicates the number of the field site (1-100) where the attack occurred. All field sites were surveyed for predation on four consecutive days. Record_date indicates the calendar date on which data was collected (format: m/dd/yy). Species refers to the facsimile species (iphiclus, serpa, or junonia), and fac_number provides a unique ID number for each facsimilie used in this experiment (i.e., 1 - 9000). Finally, attacks indicates whether each facsimile experienced an attack (0 or 1). 

- **"la_selva_site_details":** This CSV file contains additional information about the land use and trail type within each field site at La Selva Biological Station. This data is used to generate the random effect of "habitat" in the models presented at Line 193 of the "absolute_density_analysis.Rmd" script. Site_number provides the unique number associated with each field site (1-100), and density_treatment and unpalatability_treatment variables are consistent with the descriptors provided above. trail_type indicates whether the path were facsimiles were placed in the field consisted mainly of concrete, dirt, or gravel. land_use_broad provides broad descriptors of forest structure (BDG = buildings; developed areas, MF = modified forest, PF = primary forest, SF = secondary forest). land_use_specific provides more specific descriptors of forest structure, nested within the land_use_broad varaible (AA = abandoned agroforestry, AP = abandoned plantations, A = arboretum, DA = developed areas, ER = ecological reserve, OGF = old growth forest, SF = secondary forest, SLF = selectively logged forest, SP = successional plots). the land_use_broad variable was used in the final analysis. 


#R and Package Version Information: 
> R.version.string
[1] "R version 4.5.1 (2025-06-13)"
> packageVersion("curl")
[1] ‘7.1.0’
> packageVersion("ggplot2")
[1] ‘4.0.1’
> packageVersion("lme4")
[1] ‘1.1.37’
> packageVersion("lmtest")
[1] ‘0.9.40’
> packageVersion("statmod")
[1] ‘1.5.1’
> packageVersion("emmeans")
[1] ‘1.11.2.8’
> packageVersion("car")
[1] ‘3.1.3’
> packageVersion("glmmTMB")
[1] ‘1.1.13’
> packageVersion("dplyr")
[1] ‘1.1.4’
> packageVersion("DHARMa")
[1] ‘0.4.7’
> packageVersion("performance")
[1] ‘0.15.3.7’
> packageVersion("sjPlot")
[1] ‘2.9.0’
> packageVersion("sjmisc")
[1] ‘2.8.11’
> packageVersion("survival")
[1] ‘3.8.3’
> packageVersion("coxme")
[1] ‘2.2.22’
> packageVersion("survminer")
[1] ‘0.5.1’
> packageVersion("jstable")
[1] ‘1.3.23’
> packageVersion("broom")
[1] ‘1.0.10’
