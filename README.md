# Iris Flower Classification with Deep Neural Network (Keras)


##  Dataset

The Iris dataset is a classical machine learning dataset that contains:
- 150 samples
- 3 classes of iris flower: *setosa*, *versicolor*, *virginica*
- 4 numerical features: *sepal length*, *sepal width*, *petal length*, *petal width*

📥 [Download the dataset](https://www.kaggle.com/datasets/arshid/iris-flower-dataset/code) 

---

##  Goals

- Build a DNN (Deep Neural Network) classifier using **TensorFlow Keras**
- Handle model randomness with **reproducibility best practices**
- Implement **EarlyStopping** to prevent overfitting
- Track and analyze **accuracy** and **validation loss**
- Generate a **confusion matrix** for performance inspection
- Compare with a baseline **logistic regression model**

---

##  What I Tried and Learned

###  Deep Neural Network (DNN) with Keras
- Designed a Keras `Sequential` model with multiple dense layers
- Observed how adding/removing layers and changing neurons affected accuracy
- Learned that model results can vary due to **random initialization**

###  Reproducibility
- Used `set_seed()` to **fix randomness**
- Repeated training multiple times with different seeds to calculate average accuracy
- Noted how **changing only the seed** could cause results to swing from 63% to 93%

###  EarlyStopping
- Applied `EarlyStopping` with `restore_best_weights=True`
- Validated model performance using `val_loss` and `val_accuracy`
- Learned that EarlyStopping is more useful on larger or noisier datasets

###  Evaluation
- Built a **confusion matrix** to inspect how well the model performed across classes
- Compared model predictions with ground truth labels
- Printed final validation accuracy after training

---

## 🎯 Results

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression | 100% ✅ |
| Deep Neural Network | ~93% (best run), average ~85% |

---

## 📈 Tools & Libraries
- Python
- TensorFlow & Keras
- Scikit-learn
- Matplotlib
- Pandas

---

