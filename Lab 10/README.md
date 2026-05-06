# Iris Flower Classification using SVM

This project uses the famous Iris dataset to classify iris flower species using a Support Vector Machine (SVM) model.

## Dataset
The dataset contains 150 samples from three iris flower species:
- Setosa
- Versicolor
- Virginica

Features used:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## Technologies
- Python
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

## Steps
1. Load and explore the Iris dataset
2. Visualize the data using PairPlot and KDE Plot
3. Split the data into training and testing sets
4. Train an SVM classifier
5. Evaluate the model using:
   - Confusion Matrix
   - Classification Report
6. Improve the model using GridSearchCV

## Results
The SVM model achieved very high accuracy on the Iris dataset.  
GridSearchCV was used to tune parameters such as `C` and `gamma` for better performance.
