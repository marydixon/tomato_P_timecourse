# tomato-p-timecourse


## Overview

This repository contains the R code and data associated with the following manuscript:

Dixon M, Afkairin A, Manter D, Godfrey J, Hamm A, Munoz N, Bloodsworth K, 
Balasubramanium V, Buchanan C, Ippolito J A, Burnet, M, Vivanco J M.

Wild tomato responds to a flush of exogenous nutrition by interacting with its rhizosphere microbiome to maintain soluble soil phosphorous concentrations 
Code are available to reproduce the results and figures in the manuscript.  


## File descriptions

1. "Biomass.Rmd" includes code to analyze differences in dry biomass for roots and shoots of tomato in the time course trial. 
	- Data inputs:  
		- "Biomass_TimeCourse.csv": Raw dry shoot and root biomass values.       
	- Data outputs:  
		- Component of Figure 1 and results corresponding to figure 1

2. "P_Concentration_Olsen_P.Rmd" includes code to determine differences in shoot P uptake and in difference between the shoot P uptake of fertilized and unfertilized tomato. Also, we explore Olsen P differences.
	- Data inputs:  
		- "P_Concentration_Blank_Seedling.csv.csv": Phosphorus concentration (from ICP-AES) and P uptake values for shoots.  
		- "Root_P.csv": Root P concentration data
		- "Olsen-P.csv": Olsen P data
	- Outputs: 
		- "Figure1.png" Contains biomass and P data for main text fig one
		- Results corresponding to figure 1
		- Results corresponding to figure 2

3. "water_soluble_p.R" includes code to determine differences in water soluble P concentrations. 
	- Data inputs:  
		- "Olsen_P.csv": Bulk soil Olsen P concentration values.  
	- Outputs:  
		- "Figure3.pdf" Bulk soil Olsen phosphorus concentration (mg/kg) in tomato across a domestication gradient. 
		- Results corresponding to figure 3
		
4. "Mehlich_Total_P.R" includes code to assess mehlich 3 data
	- Data inputs:  
		- "Soil_M3_Total.csv": Includes Mehlich 3 data  
	- Outputs:  
		- Results corresponding to figure 2
4. "P_cycling_bacteria.rms" includes code to assess rhizosphere P solubilizers. 
	- Data inputs:  
		- "EMU_database.GIBBs.KO.PICRUST2.xlsx": contains picrust2 data
		- "P.Time.rel.RDS": relative abundance 
	- Outputs:  
		- Results corresponding to figure 3
		
5. "P_cycling.R" includes code to determine different bacterial species that change in abundance between treatments.
	- Data inputs:  
		- "Phyloseq.Count.Data.RDS": phyloseq object showing bacterial abundance count data (culled from code in "Microbiome_Read_In_Data")
	- Outputs:  
		- "Figure5.pdf.pdf" Differential abundance (DA) analysis showing the log fold change in bacteria abundance between different domestication and varietal groups. 
		- Results corresponding to Figure 5

6. "qPCR.Rmd" includes code to analyze the microbial biomass 
  - Data inputs:
		- "qPCR.csv": contians qpcr data
	- Outputs:  
	  - results corresponding to figure 3
7. "diff_abund_function.Rmd": includes code to determine microbial fluctuations
  - Data inputs
    - "EMU_database.GIBBs.KO.PICRUST2.xlsx": Picrust2 data similar to above
    - "P.Time.RDS": Bacterial count data
  - Data outputs
    - Results corresponding to figure 4
    - Information for supplemental tables comprising data for differential abundance analyses
8. "GC_LC_MS.Rmd": analyzing metabolomics data
  - Data inputs 
    - "lcms_61157_tomato_results_rp_pos.csv": LCMS RP Positive data
    - "lcms_61157_tomato_results_rp_neg.csv": LCMS RP Negative data
    - "lcms_61157_tomato_results_hilic_pos.csv": LCMS HILIC Positive data
    - "lcms_61157_tomato_results_hilic_neg.csv" LCMS HILIC Negative data
    - "gcms_61157_tomato_results_Sp.csv": GCMS data
  - Data outputs
    - Results corresponding to figure 5
9. "P_Assay.Rmd": Analyzes P solubilization index\
 - Data inputs
    - "P_Sol.csv": Has PSI data 
 - Data outputs
    - results correspondong to figure 6
10. "biomass_psf": Assess biomass data for the cylces experiment
 - Data inputs
    - "Biomass_psf.csv": Has biomass data for the cycles experiment
 - Data outputs
    - results corresponding to figure 7 
11. "Root_P.Rmd": Has code for looking at the root P uptake and concentration for the cycles trial
 - Data inputs
    - "Root_P.csv" Contains root P data
 - Data outputs
    - results corresponding to figure 7
12. "p_cycling_bacteria_Cycles.Rmd": Includes code to compare the P decomposer and solubilizer relative abundacne in the third cyclestrial
 - Data inputs
    - "P.rel.Cycles.RDS": Relative abundance data as a phyloseq object
 - Data outputs 
    - Results corresponding to figure 7 
    - Supplementary figure 7 
13. "Olsen_P_Cycles.Rmd"
 - Data inputs
    - "Olsen_P_Cycles.csv": Contains olsen p data for the cycles exp
 - Data outputs 
    - Results corresponding to figure 7