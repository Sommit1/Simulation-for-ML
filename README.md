# Data Generation using Modelling and Simulation for Machine Learning (SIR Model)

This repository contains an assignment implementation for data generation using simulation and applying machine learning models on the generated dataset. The simulation is based on the SIR (Susceptible–Infected–Recovered) epidemic model, and 1000 simulations were generated to create a synthetic dataset.

# Methodology

1. Simulation Model Used

The SIR model divides the population into:

S(t): Susceptible

I(t): Infected

R(t): Recovered

2. Parameter Bounds

Random values were generated within the following bounds:

Parameter                	Range
β (beta)                	0.1 – 1.5
γ (gamma)                	0.05 – 0.5
Population(N)            	500 – 5000
Initial Infected(I0)    	1 – 50
Days                    	80 – 200

3. Data Generation (1000 Simulations)

For each simulation, random parameters were sampled and the SIR model was executed. Important outputs were recorded such as:

Peak infected fraction

Time to peak infection

Final recovered fraction

R0 value (β/γ)

Dataset saved as:

simulations_1000.csv

4. Target Label (Classification)

A binary label was created:

Severe outbreak = 1 if peak infected fraction > 0.10

Non-severe outbreak = 0 otherwise

# Result Graphs

Peak Infected Fraction Distribution

<img width="1087" height="576" alt="peak_distribution" src="https://github.com/user-attachments/assets/5411b775-10a4-4bb2-a439-76bea25160b3" />

Severe vs Non-Severe Class Balance

<img width="722" height="518" alt="class_balance" src="https://github.com/user-attachments/assets/e5fb40a1-6834-490a-beec-9111108dab49" />

# Machine Learning Models Used

The dataset was used to train multiple classification models:

Logistic Regression

-Random Forest

-Gradient Boosting

-SVC

-KNN

-Decision Tree

-MLP

Evaluation metrics used:

-Accuracy

-Precision

-Recall

-F1 Score

-ROC-AUC

# Model Comparison Table

<img width="381" height="322" alt="image" src="https://github.com/user-attachments/assets/30ab829e-afee-4ccc-9ea9-97861a518a91" />

# Best Model

Decision Tree Classifier performed best with perfect performance:

Accuracy = 1.00

F1 Score = 1.00

# Author

Sommit
