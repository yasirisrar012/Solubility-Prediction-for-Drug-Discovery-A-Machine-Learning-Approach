# Solubility Prediction for Drug Discovery : A Machine Learning Approach  

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
- **Linear Regression Performs Better Overall**: It achieves lower MSE and higher R² on the test set, indicating better generalization compared to Random Forest.
- **Random Forest Shows Signs of Overfitting**: The Test MSE for Random Forest is significantly higher than its Training MSE, suggesting it might be overfitting the training data.
- **Complexity vs Simplicity**: Random Forest, being a more complex model, might not always outperform simpler models like Linear Regression on smaller datasets or when the relationships between features and the target are relatively linear.

## Applications in the Pharmaceutical Industry  
This project demonstrates the potential of machine learning in solving real-world problems such as:  
- Early-stage drug discovery by predicting solubility for large compound libraries.  
- Optimization of drug formulations based on solubility insights.  
- Reducing experimental costs by prioritizing computational predictions.  
