# Day 3 - ML Pipeline with GitHub Actions

This project is a basic Machine Learning pipeline created for Day 3 practice.
It uses the Iris dataset from Scikit-learn and follows a simple pipeline structure:

1. Load dataset
2. Preprocess data
3. Train model
4. Evaluate model
5. Run tests
6. Automate workflow using GitHub Actions

## Project Structure

```txt
day3_pipeline/
│
├── data_loader.py
├── preprocess.py
├── train.py
├── evaluate.py
├── main.py
├── requirements.txt
├── test_pipeline.py
│
└── .github/
    └── workflows/
        └── day3-pipeline.yml
```

## Technologies Used

* Python
* Scikit-learn
* Pytest
* Flake8
* Git
* GitHub Actions

## Dataset

This project uses the built-in Iris dataset from Scikit-learn.

The Iris dataset contains flower measurements and is commonly used for classification tasks.

## How the Pipeline Works

### 1. Data Loading

The dataset is loaded using `load_iris()` from Scikit-learn.

### 2. Data Preprocessing

The data is split into training and testing sets using `train_test_split`.

### 3. Model Training

A Random Forest Classifier is trained on the training data.

### 4. Model Evaluation

The trained model is tested on test data and accuracy is calculated.

### 5. Testing

Pytest is used to check whether the dataset loads correctly.

### 6. CI/CD Workflow

GitHub Actions automatically runs the following steps whenever code is pushed:

* Checkout code
* Setup Python
* Install dependencies
* Run linter
* Run tests
* Execute ML pipeline

## Installation

Install all required dependencies:

```bash
pip install -r day3_pipeline/requirements.txt
```

## Run the ML Pipeline

```bash
python day3_pipeline/main.py
```

## Run Tests

```bash
pytest day3_pipeline/test_pipeline.py
```

## GitHub Actions Workflow

The workflow file is located at:

```txt
.github/workflows/day3-pipeline.yml
```

The workflow runs automatically on every push to GitHub.

## Output

After running the pipeline, the model accuracy is printed:

```txt
Model Accuracy: 1.00
```

## What I Learned

In this project, I learned:

* How to create a basic ML pipeline
* How to split code into multiple Python files
* How to use Scikit-learn
* How to write basic tests using Pytest
* How to use Flake8 for code checking
* How to automate a pipeline using GitHub Actions
* How to push a project from VS Code to GitHub
