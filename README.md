# Quantifying Untargeted Metabolomics

This is the GitHub for the paper, "Estimating nutrient concentration in food using untargeted metabolomics," where we use the universal scaling of nutrient concentrations discussed previously in [1] to quantify the concentrations of compounds in untargeted metabolomics experiments. 

## Data Folder

Contains all the data used within the paper. 

- **USDA_plant_only**: The raw USDA - Standard Reference data for all raw foods identified as plants with minimal processing.
- **USDA_filtered_to_experiments**: The raw USDA data for the foods used within the experiments, from Standard Reference and Foundation Foods.
- **USDA-MS-Overlap_Data**: Data for the compounds in overlap between the USDA, providing concentrations, and our MassSpec experiments, providing peak areas. 
- **USPX_features**: Compound-Food pairs for all raw plants within the USDA and Phenol Explorer, containing the calculated chemical properties for each compound and the phylogenetic tree information for each food. This is the training data for the ML model.
-  **MassSpec_features**: The chemical properties and phylogenetic tree information for all compounds and foods within the MassSpec experiments.
-  **FoodMine_features**: The chemical properties and phylogenetic tree information for select compounds and foods scraped from the scientific literature using FoodMine [2]. This is used to predict the concentration of compounds in MassSpec that are not reported in the USDA.

## Code Folder

- **USPX model prediction**: The code for the model trained on the USPX data as presented in the paper. Predicts the concentrations for untargeted metabolomics using peak areas for compounds reported and unreported in the USDA.  
- **USPX Model Leave-One_Out**: The leave-one-out validation code used to support the model within the paper.

### References
[1] Menichetti, G. & Barabasi, A.-L. Universal scaling of nutrient concentrations in food. Nat. Food 1–66 (2021).

[2] Hooton, F., Menichetti, G. & Barabási, A.-L. Exploring food contents in scientific literature with FoodMine. Sci. Rep. 10, 16191 (2020).

# Paper Citation

Sebek, M., Menichetti, G., & Barabási, A.-L. Estimating nutrient concentration in food using untargeted metabolomics. (2022).
