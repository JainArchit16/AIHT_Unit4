# Air Quality Classification in Indian Cities with PySpark

A PySpark-based machine learning pipeline to classify air quality categories in Indian cities using the ["Air Quality Data in India" dataset](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india?select=city_day.csv). The project demonstrates scalable data preprocessing, feature engineering, model training (Random Forest), evaluation, and visualization of results—all in a reproducible notebook format.

---

## Table of Contents

- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Directory and File Overview](#directory-and-file-overview)
- [Contribution Guidelines](#contribution-guidelines)
- [License](#license)
- [Credits](#credits)
- [Contact](#contact)
- [Badges](#badges)

---

## Features

- **Automated Data Download:** Fetches the latest air quality dataset from Kaggle.
- **PySpark Integration:** Uses Spark for scalable data processing and machine learning.
- **Data Cleaning & Feature Engineering:** Handles missing values, type conversions, and vectorization.
- **Classification Pipeline:** Implements a Random Forest classifier to predict AQI buckets.
- **Model Evaluation:** Reports accuracy, confusion matrix, and error metrics.
- **Hyperparameter Tuning:** Utilizes cross-validation and grid search for optimal model selection.
- **Visualization:** Plots confusion matrix for model diagnostics.
- **Reproducibility:** All steps are contained within a single, annotated Jupyter notebook.

---

## Dataset

- **Source:** ["Air Quality Data in India" by Rohan Rao on Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india?select=city_day.csv)
- **File Used:** `city_day.csv`
- This dataset contains daily air quality and pollutant measurements for major Indian cities.

---

## Installation

1. **Clone the Repository:**

```
git clone https://github.com/yourusername/air-quality-pyspark.git
cd air-quality-pyspark

```

2. **Install Dependencies:**

- Python 3.7+
- [PySpark](https://spark.apache.org/docs/latest/api/python/)
- [findspark](https://github.com/minrk/findspark)
- [kagglehub](https://github.com/KaggleHub/kagglehub)
- [matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
- [scikit-learn](https://scikit-learn.org/)

Install via pip:

```
pip install pyspark findspark kagglehub matplotlib pandas scikit-learn

```

3. **Kaggle API Setup:**

- Place your `kaggle.json` in the appropriate location as per [Kaggle API instructions](https://github.com/KaggleHub/kagglehub).

---

## Usage

Open and run the notebook:

```
jupyter notebook spark.ipynb
```

The notebook will:

- Download the dataset from Kaggle.
- Initialize Spark and load the data.
- Clean and preprocess the data.
- Build and train a Random Forest classifier.
- Evaluate and visualize the results.

**Example:**  
To run the pipeline, execute all cells in the notebook sequentially.  
Key outputs include model accuracy, confusion matrix, and best hyperparameters found via cross-validation.

---

## Project Structure

```
air-quality-pyspark/
│
├── spark.ipynb # Main Jupyter notebook with the entire pipeline
├── README.md # Project documentation
├── LICENSE # Project license (MIT)
└── requirements.txt # (Optional) List of Python dependencies
```

---

## Directory and File Overview

- `spark.ipynb`: Main notebook containing the full PySpark pipeline, from data ingestion to evaluation and visualization.
- `README.md`: This documentation file.
- `LICENSE`: Project license.
- `requirements.txt`: (Optional) List of Python dependencies.

---

## Contribution Guidelines

Contributions are welcome! To contribute:

- Fork this repository.
- Create a new branch (`git checkout -b feature/your-feature`).
- Commit your changes (`git commit -am 'Add new feature'`).
- Push to the branch (`git push origin feature/your-feature`).
- Open a Pull Request.

Please follow [PEP 8](https://pep8.org/) coding standards and include clear documentation/comments.

---

## Credits

- [Rohan Rao](https://www.kaggle.com/rohanrao) for the [Air Quality Data in India dataset](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india?select=city_day.csv).
- [Apache Spark](https://spark.apache.org/), [PySpark](https://spark.apache.org/docs/latest/api/python/), and open-source contributors.
- [KaggleHub](https://github.com/KaggleHub/kagglehub) for dataset management.

---

## Contact

For questions, suggestions, or collaboration, please contact:

- **Your Name**
- **Email:** your.email@example.com
- **GitHub:** [yourusername](https://github.com/yourusername)

---

## Badges

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

_Ready to scale air quality analytics with big data tools and open science!_

---

**Note:**  
If you need to customize dataset paths, Spark configuration, or want to add new models, please refer to the code comments in `spark.ipynb`.  
If any project-specific details (such as author name, email, or repository URL) need to be updated, please replace the placeholders above.
