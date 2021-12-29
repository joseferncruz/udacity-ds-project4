# Recommendation systems with IBM
---

**[Udacity Nanodegree in Data Science](https://www.udacity.com/course/data-scientist-nanodegree--nd025) - Project 4**


🏗️ In this project I **built 3 types of recommendation systems** using User-Article interactions from IBM Watson platform **based on**:

- **Rank** (on total article interactions)
- **Collaborative Filtering**:
    - **Neighborhood Based Recommender**  (User-User interactions)
    - **Model Based Recommender - Matrix Factorization** (User-Item interactions)



To achieve this goal I used:
- ✅**python3 - numpy, pandas and matplotlib**:
  - Data cleaning and data wrangling,
  - Descriptive statistics,
  - Visualization techniques,
  - Linear algebra operations for matrix factorization

If you have any **questions** or **suggestions**, just send me a 💬 via [**LinkedIn**](https://www.linkedin.com/in/josecruz-phd/). **Enjoy!**


## Table of Contents

- [Introduction](#introduction)
- [Repository content](#repository-content)
- [The data](#the-data)
- [Requirements](#requirements)
- [The recommendation systems](#the-webapp)
- [Licensing and Acknowledgements](#licensing-and-acknowledgements)


## 📖 Introduction


The need for recommendation systems is a key foundation in many modern businesses. A quick interaction with several online platform (eg Amazon, Facebook, Google Search, etc) show us that everyday suggestions are not entirely random but are rather personalized to each user. For instance, Netflix suggests movies to users based on their view history, their connections, demographics and many other features.

**The more relevant the recommendation, but higher engagement the service will generate.**

Thus, having ways to build robust recommenders that can provide novel, useful, relevant and diverse recommendations is a key objective to business that aim to provide personalized services.

In this project, I used data provided by IBM Watson studio on interactions between users and platform articles they interact with. The object was to build a recommendation system that could suggest new articles to users based on different strategies.


## 📂 Repository content

    - data
    | - articles_community.csv
    | - user_item_matrix.p
    | - user-item-interactions.csv

    - tests
    |- project_tests.py

    - README.md
    - LICENSE
    - Recommendations_with_IBM.ipynb
    - .gitignore
    - environment.yml


## 📊 The data

The dataset was provided by IBM Watson Studio and was made available by Udacity content creators.

The `articles_community.csv` contains information about the individual articles:

 | Column       |  Data type  |
 | --------------- | -----|
 | doc_body        |  str |
 | doc_description |  str |
 | doc_full_name   |  str |
 | doc_status      |  str |
 | article_id      |  int |

The `user-item-interactions.csv` contains information about the interaction between users and articles.


| Column   |  Data type  |
| -------------| -----|
| article_id   |  int |
| title        |  str |
| email        |  str |

 "email" **does not** contain personally identifiable information.


## 🔨 Requirements

To use the python scripts on your local machine, you need to:

1. Install a python environment with jupyter notebooks (e.g., [anaconda distribution](https://www.anaconda.com/products/individual)).

2. Create an environment with the required packages by running on the anaconda shell:
```
conda env create -f environment.yml --name myenv
conda activate myenv
jupyter lab Recommendations_with_IBM.ipynb
```


## 💻 Recommendations with IBM

In the notebook `Recommendations_with_IBM.ipynb` you can find 5 sections:

#### I. Exploratory Data Analysis
Descriptive statistics and basic visualization techniques to understand the data.

#### II. Rank Based Recommendations
First recommendation system based on popularity of the articles accross users.

#### III. User-User Based Collaborative Filtering
Second recommendation system based on similarities between users and the articles they interacted with.

#### IV. User-Article Matrix Factorization
Third recommendation system created by using Single Value Decomposition on User-Article interactions.

#### V. Conclusions, Actions and Future Directions
Discussion about the performance of the recommendation systems, drawbacks of implementations, actionable items and future directions.


## 📃 Licensing and Acknowledgements

The analysis and code generated during this project are licensed under a MIT License.

I would like to thank [Udacity](https://www.udacity.com/) for providing the content of the project.

---
2021, [José Oliveira da Cruz](https://www.linkedin.com/in/josecruz-phd/)
<h4 id="disclaimer">Disclaimer</h4>
 The author is not affiliated with any of the entities mentioned nor received any kind of compensation. The information contained in this work is provided on an "as is" basis with no guarantees of completeness, accuracy, usefulness or timeliness.
