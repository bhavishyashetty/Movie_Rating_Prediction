# Movie Rating Prediction 🎥⭐  

## Overview  
This project predicts movie ratings based on features such as **year of release**, **duration**, **genre**, **votes**, and key contributors (director and main actors). Using **Random Forest Regressor** as the primary regression model, the project demonstrates feature preprocessing, encoding, and evaluation of model performance.  

---

## Dataset  
The dataset contains the following columns:  
1. **Name**: Title of the movie.  
2. **Year**: Year of release.  
3. **Duration**: Runtime of the movie in minutes.  
4. **Genre**: Primary genre of the movie (e.g., Action, Comedy, Drama).  
5. **Rating**: IMDb rating (target variable, scale of 1–10).  
6. **Votes**: Number of votes received on IMDb.  
7. **Director**: Name of the director.  
8. **Actor 1**: Name of the lead actor.  
9. **Actor 2**: Name of the second main actor.  
10. **Actor 3**: Name of the third main actor.  

---

## Objective  
The goal is to build a machine learning model that accurately predicts movie ratings based on input features, with a focus on achieving low prediction error and high interpretability.  

---

## Workflow  

### 1. **Data Preprocessing**  
- Encode categorical features such as `Genre`, `Director`, and `Actors` using **OneHotEncoder**.  
- Standardize numerical features like `Year`, `Duration`, and `Votes` using **StandardScaler**.  

### 2. **Feature Engineering**  
- Combine numerical and encoded categorical features for model training.  
- Split the data into **training** and **testing** sets.  

### 3. **Modeling**  
- Train a **Random Forest Regressor**, a robust ensemble-based regression model.  
- Use 100 decision trees with default hyperparameters.  

### 4. **Evaluation**  
- Measure model performance using:  
  - **Mean Squared Error (MSE)**: Average squared difference between actual and predicted ratings.  
  - **R² Score**: Proportion of variance explained by the model.  

---

## Results  
- **Model**:  1.6158   
- **Metrics**:  
  - **Mean Squared Error (MSE)**: 0.1274
  - **R² Score**: 5.11

---

## Setup  

### Prerequisites  
Ensure you have Python ≥3.8 installed along with the following libraries:  
```bash  
pip install numpy pandas scikit-learn  
```  

### Steps to Run  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/bhavishyashetty/Movie_Rating_Prediction.git
   cd Movie_Rating_Prediction  
   ```  
2. Place your dataset in the project directory as `IMDb Movies India.csv`.  
3. Run the script in your Python environment (e.g., Jupyter Notebook, VS Code).  


