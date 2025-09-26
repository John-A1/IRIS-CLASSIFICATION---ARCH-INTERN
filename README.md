# IRIS-CLASSIFICATION---ARCH-INTERN

# 🛠️ Training a Neural Network on the Iris Dataset  

This project demonstrates how to train a **Neural Network (using TensorFlow/Keras)** on the classic **Iris dataset** to classify flower species.  
We explore **loss behavior (categorical cross-entropy)** and track **accuracy** across training epochs.  


## 📌 Objective  
- Train a neural network to classify **Iris flower species**.  
- Observe the behavior of the **categorical cross-entropy loss** function during training.  
- Visualize **loss and accuracy curves** for both training and validation sets.  

---

## 📊 Dataset  
The [Iris dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html) is a well-known dataset in machine learning, consisting of:  

- **150 samples** of iris flowers  
- **4 features**: sepal length, sepal width, petal length, petal width  
- **3 classes**: *Iris-setosa, Iris-versicolor, Iris-virginica*  

---

## ⚙️ Project Workflow  

### **1. Import Libraries & Load Data**  
- Load the Iris dataset from `sklearn`.  
- Perform **one-hot encoding** on labels.  
- Standardize features using `StandardScaler`.  
- Split into **train (80%)** and **test (20%)** sets.  

### **2. Build Neural Network Model**  
The model is a **Sequential neural network** with:  
- Dense(32, ReLU) → Dense(64, ReLU) → Dense(32, ReLU) → Dense(16, ReLU)  
- Dense(3, Softmax) for output (3 classes)

### **3. Train the Model**  
- **Epochs:** 50  
- **Batch size:** 8  
- Training and validation performance tracked.  

### **4. Plot Loss & Accuracy**  
- Training vs validation **loss curves**  
- Training vs validation **accuracy curves**  

---

## 📈 Results & Interpretation  
✅ **Loss decreases with epochs**, indicating the network is learning effectively.  
✅ **Validation accuracy stabilizes**, showing good generalization.  
⚠️ If validation loss diverges from training loss → potential **overfitting**. 
- Optimizer: **Adam**  
- Loss: **Categorical Crossentropy**  
- Metric: **Accuracy**  
