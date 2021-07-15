## Week 2 
### Assignment 

- [Notes on data and model management with DVC](https://www.notion.so/Week-2-Data-Model-Management-with-DVC-1bdbe182a0d344cca193c9cdb7e18a64)
- [Github repository containing assignment on DVC](https://github.com/shriishwaryaa/MLOps_Assignment/tree/main)

<hr>

### Questions

***List the commands (in sequence) that you used to accomplish the tasks mentioned in Part 1 of the assignment***

File structure :-

```bash
Desktop
└── external_cache
└── MLOps_assignment
    ├── .dvc
    ├── .dvcignore
    ├── .git
    ├── data
    │   └── .gitignore
    │   └── creditcard.csv
    │   └── creditcard.csv.dvc
    │   └── prepared
    │       └── test.csv
    │       └── test.csv.dvc
    │       └── train.csv
    │       └── train.csv.dvc
    ├── metrics    
    │   └── .gitignore
    │   └── acc_f1.json
    │   └── acc_f1.json.dvc
    ├── models
    │   └── .gitignore
    │   └── model.pkl 
    │   └── model.pkl.dvc
    ├── README.md
    └── src
        └── expt.py
```

Terminal commands :-

```zsh
cd Desktop
mkdir MLOps_Assignment 
cd MLOps_Assignment  

git init
git remote add origin https://github.com/shriishwaryaa/MLOps_Assignment.git
git pull origin main
git branch -M main
dvc init

mkdir data
cd ..
mkdir external_cache
cd MLOps_Assignment 
dvc cache dir ../external_cache

dvc add data/creditcard.csv
git add data/creditcard.csv.dvc data/.gitignore
git commit -m "Added raw data"

dvc remote add -d storage s3://mlopsassignment180100112/datastore/
git add .dvc/config
git commit -m "Configured remote storage"

git push origin main
dvc push
```

<hr>

***List the values of Accuracy & Weighted F1 Score obtained from both the experiments conducted in Part 2 of the assignment***

| Model            |   Accuracy           | Weighted F1 Score    |
| :---:            |     :----:           |         :---:        |
| Decision Tree    | 0.9993679997191109   | 0.9993679997191109   |
| Random Forest    | 0.9996313331694814   | 0.9996224760940732   |

<hr>

***AWS S3 bucket***

![Week2 bucket](/Images/aws_week2_bucket.png)
