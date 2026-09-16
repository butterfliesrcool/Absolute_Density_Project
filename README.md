# Code for: Increasing absolute prey density within a mimicry complex protects aposematic models and their Batesian mimics 

**Corresponding Author:** Abigail E. Robinson 

**Abstract:** Batesian mimicry is a defensive adaptation where predators learn to avoid aposematic prey and generalize their warning signals to phenotypically similar mimics. The phenotypic accuracy needed for mimics to benefit from this generalization depends on the relative densities of models and mimics and the model’s unpalatability. As aposematic models become more unpalatable or more common relative to their mimics, warning signals become stronger, allowing even poor mimics to gain protection. However, few studies have disentangled the importance of the relative frequency of models and mimics from the absolute density of the prey community (both models and mimics) in driving relaxed selection on imperfect mimics. Here, we test the hypothesis that increasing model unpalatability and absolute density of the prey community accelerates predator avoidance learning and enhances protection for imperfect mimics. Using replicas of the model Adelpha iphiclus (Linnaeus), its imperfect mimic Adelpha serpa (Boisduval), and the palatable control Junonia evarete (Cramer), we conducted field experiments that enhanced model unpalatability and doubled absolute prey density while maintaining a constant ratio of model, mimic, and control phenotypes. We found that enhanced model unpalatability and increased absolute density of the mimicry complex significantly reduced predation on all species, highlighting absolute community density as an underappreciated mechanism shaping selection on imperfect Batesian mimics.

- **"absolute_density_analysis.Rmd":** This R Markdown file contains the code for fitting GLMMs and Cox Proportional Hazards models to predation data from our field experiments, including data cleaning, model selection, and visualization of results.

Within the **data_files** folder:

- **"density_dependence_binomial_data.csv":** This CSV file contains the raw data collected from the field experiments, including information on predation events, species identity, treatment groups, and other relevant variables. For unpalatability variable, "no" indicates that model unpalatability was not experimentally enhanced with a 2% Bitrex solution, while "yes" indicates that model unpalatability was enhanced with the Bitrex solution. For density variable, "low" indicates that a given field site was under low asbolute prey density conditions (i.e., 20 facsimilies / species), while "high" indicates that a given field site was under high absolute prey density conditions (i.e., 40 facsimilies / species).

- **"density_data_fac_no.csv":** This CSV file contains all data as described for the **density_dependence_binomial_data.csv** file, except a unique number is given to each facsimile used in the experiment (i.e., 1 - 9000), rather than repeating facsimile numbers across sites. This data file was used in the final analysis.

- **"la_selva_site_details":** This CSV file contains detailed information about the land use and trail type within each field site 

- **"la_selva_site_details_simple":** This CSV file contains simplified information about land use (primary, secondary, or modified forest or buildings, to indicate sites in developed parts of the reserve)


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
