# Molecular Solubility Prediction with Machine Learning  

## Project Overview  
This project focuses on predicting the aqueous solubility (**logS**) of chemical compounds using molecular descriptors and machine learning techniques. The dataset utilized includes molecular features such as `MolLogP`, `MolWt`, `NumRotatableBonds`, and `AromaticProportion`. Two machine learning models, **Linear Regression** and **Random Forest**, are implemented and compared to evaluate their predictive performance.  

The project is particularly relevant for applications in the **pharmaceutical industry**, where solubility prediction is critical for drug design, development, and optimization.  

## Dataset  
The dataset used is the **Delaney Solubility Dataset**, which provides solubility values (`logS`) along with molecular descriptors for various chemical compounds.  
### Key Features:  
- **MolLogP**: Octanol-water partition coefficient (logP).  
- **MolWt**: Molecular weight of the compound.  
- **NumRotatableBonds**: Number of rotatable bonds in the molecule.  
- **AromaticProportion**: Proportion of aromatic atoms in the molecule.  
- **logS**: Logarithmic value of aqueous solubility (target variable).  

## Tools I Used  
- **Programming Language**: Python  
- **Libraries**:  
  - **Scikit-Learn**: Machine learning model implementation.  
  - **Pandas**: Data manipulation and preprocessing.  
  - **NumPy**: Numerical computations.  
  - **Matplotlib** & **Seaborn**: Data visualization.  

## Project Workflow  
### 1. **Data Preprocessing**  
- Load and clean the dataset.  
- Feature selection and exploration of relationships between descriptors and **logS**.  

### 2. **Modeling**  
- **Linear Regression**: A baseline model to establish performance on the dataset.  
- **Random Forest Regressor**: A non-linear model to capture complex relationships in the data.  

### 3. **Evaluation**  
- Compare the models using evaluation metrics:  
  - **Mean Squared Error (MSE)**  
  - **R² Score**  
- Visualize predictions vs actual values for both models.  

## Results and Insights  
- **Linear Regression**: Provides a baseline performance but struggles with non-linear relationships.  
- **Random Forest**: Achieves higher accuracy due to its ability to capture complex patterns in the data.  
- **Feature Importance**: Analysis reveals the impact of each descriptor on solubility predictions.  

## Applications in the Pharmaceutical Industry  
This project demonstrates the potential of machine learning in solving real-world problems such as:  
- Early-stage drug discovery by predicting solubility for large compound libraries.  
- Optimization of drug formulations based on solubility insights.  
- Reducing experimental costs by prioritizing computational predictions.  
