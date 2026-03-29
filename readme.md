# Intelligent Tax Planning Advisory Agent

**Course:** CS336 Artificial Intelligence and Machine Learning (AIML)
**Section:** B.Tech VI Semester - CSE (section-C)

## Overview
This repository contains an AI-driven Intelligent Tax Planning Advisory Agent designed to assist users with tax liability estimation and deductions. The agent uses rule-based modeling on synthetic tax data to perform scenario analysis, estimate taxes, and provide actionable financial recommendation logic. 

## Software Environment & Requirements
To ensure compatibility and reproduce the results, please use the following software environment:
* **Python Version:** Python 3.9 or higher
* **Jupyter Environment:** Jupyter Notebook or JupyterLab

**Required Python Libraries:**
* `pandas` (Data manipulation)
* `numpy` (Numerical operations)
* `scikit-learn` (Machine learning and scaling)
* `matplotlib` (Static visualizations)
* `seaborn` (Statistical data visualization)

You can install the required dependencies using pip:
`pip install pandas numpy scikit-learn matplotlib seaborn`

## Required Execution Order
To successfully run the agent and generate the required datasets and visualizations, the five Jupyter notebooks must be executed in the following sequential order:

1. **`1_Data_and_Preprocessing.ipynb`**
   * **Purpose:** Generates the `synthetic_tax_data.csv` file containing simulated user profiles, incomes, and standard deductions. Must be run first to provide data for subsequent scripts.

2. **`2_Agent_workflow.ipynb`**
   * **Purpose:** Houses the core `TaxAdvisoryAgent` class. It performs the rule-based tax estimation, applies deduction logic, and outputs tailored recommendations for the user.

3. **`3_Unsupervised_modelling.ipynb`**
   * **Purpose:** Ingests the synthetic data, scales the financial features, and applies K-Means clustering to group taxpayers into distinct financial profiles. Outputs `clustered_tax_data.csv`.

4. **`4_Analysis.ipynb`**
   * **Purpose:** Reads the clustered dataset to generate visual interpretations, including scatter plots of income vs. investments and boxplots of medical deductions by cluster profile.

5. **`5_Interpretation.ipynb`**
   * **Purpose:** Discusses the societal impact of the model, addresses potential biases in the synthetic data, and evaluates the ethical responsibilities of deploying an automated tax advisory agent.

## How to Use the Code
1. Clone this repository to your local machine.
2. Ensure your Python environment meets the required versions and libraries listed above.
3. Launch Jupyter Notebook in the repository's root directory.
4. Open and run the notebooks strictly in the numbered order provided above. Ensure that each notebook executes completely before moving to the next, as CSV outputs from earlier notebooks are required as inputs for later ones.