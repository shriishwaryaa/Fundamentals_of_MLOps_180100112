## Week 3

### Assignment

 - [Notes on experimentation with ML pipelines using PyCaret](https://www.notion.so/Week-3-Experimentation-with-ML-Pipelines-using-PyCaret-49a475b455a2473ca65c2f3c0db4cc5e)
 - [Github repository containing assignment on PyCaret](https://github.com/shriishwaryaa/MLOps_Assignment/tree/pycaret_expt1)

<hr>

### Questions

***List the preprocessing & feature engineering techniques applied to the dataset***

- Split the data into training (& validation) and test set
- Set `train_size=0.8` so 80% is training data & 20% is held-out validation data 
- Normalize the data using the `minmax` method
- Set `polynomial_features=True` and `trigonometry_features=True` as explained in the notes
- The feature `polynomial_degree=2` set at its default value
- Set `fix_imbalance=True` to address the skew in the dataset


<hr>

***F1 Scores of top 5 models before & after fine-tuning***

| Model                        | Before fine-tuning   | After fine-tuning    |
| :---                         |     :----:           |         :---:        |
| Extra Trees Classifier       | 0.8021               | 0.8233               |
| Random Forest Classifier     | 0.6825               | 0.7162               |
| Gradient Boosting Classifier | 0.6034               | 0.7948               |
| Ada Boost Classifier         | 0.5395               | 0.7065               |
| K Neighbors Classifier       | 0.4852               | 0.7049               |

<hr>

***Precision-Recall plot***

![Precision-Recall plot](/Images/Precision-Recall&#32;plot.png)

<hr>

***Confusion matrix***

![Confusion matrix](/Images/Confusion&#32;matrix.png)

<hr>

***Report the Accuracy, Precision, Recall and F1 Score of the blended model on the unseen test dataset***

|                 | Value |
| :---            | :---: |
| Accuracy        | 1.0   | 
| Precision       | 1.0   |
| Recall          | 1.0   |
| F1 Score        | 1.0   |
