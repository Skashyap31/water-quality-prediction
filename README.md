# water-quality-prediction
Overview
This project predicts whether a sample of water is safe for drinking (potable) using machine learning techniques. It is developed as part of the Edunet-AICTE Internship Program.

We apply data cleaning, preprocessing, and classification techniques to build an accurate model that can classify water quality based on various chemical and physical properties.

📂 Dataset Information
The dataset contains features such as:

Feature	Description
pH	Acidity/alkalinity of water
Hardness	Concentration of calcium and magnesium
Solids	Total dissolved solids in ppm
Chloramines	Disinfectant level
Sulfate	Sulfate concentration
Conductivity	Electrical conductivity of water
Organic_carbon	Organic content
Trihalomethanes	Toxic compounds formed during chlorination
Turbidity	Clarity of water
Potability	Target (1 = drinkable, 0 = not drinkable)

ML Pipeline
1. Load and Inspect Dataset
2. Handle Missing Values (Imputation)
3. Remove Duplicates
4.Feature Scaling (Standardization)
5. Train-Test Split
6.Train Random Forest Classifier
7.Predict and Evaluate

