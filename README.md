# Personalized Recommendation System for Airbnb Data

## Overview
This project focuses on building a personalized recommendation system for Airbnb listings using the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology. The aim is to leverage historical data to make individualized recommendations for users, improving customer satisfaction and increasing sales. The project involves data collection, data preparation, model building, and evaluation using various clustering algorithms.

## Table of Contents
- [Overview](#overview)
- [Project Objectives](#project-objectives)
- [Business Success Criteria](#business-success-criteria)
- [Technologies Used](#technologies-used)
- [Project Workflow](#project-workflow)
  - [1. Business Understanding](#1-business-understanding)
  - [2. Data Understanding](#2-data-understanding)
  - [3. Data Preparation](#3-data-preparation)
  - [4. Modeling](#4-modeling)
  - [5. Evaluation](#5-evaluation)
- [Challenges and Limitations](#challenges-and-limitations)
- [Next Steps](#next-steps)
- [References](#references)

## Project Objectives
The main objective of this project is to improve sales by making personalized recommendations to users based on their past behavior on the Airbnb platform. The goal is to increase customer engagement by recommending listings that are aligned with their preferences.

## Business Success Criteria
To determine the success of the project, the following criteria are defined:
- Increase in sales by 8-10% within one year.
- Increase the time spent and pages viewed on the site by 5-10% within one year.
- Adhere to the allocated budget and timeline.

## Technologies Used
- **Programming Languages**: Python
- **Libraries**: Scikit-learn, Pandas, NumPy, Matplotlib
- **Tools**: Google Colab, Microsoft Office, SQL
- **Data Source**: Airbnb dataset (Listings.csv, Reviews.csv)

## Project Workflow

### 1. Business Understanding
The project starts with a clear understanding of the business goals and objectives. In this phase, we align the recommendation system's goal with Airbnb's core objective: improving user experience and increasing sales by personalizing recommendations.

#### Key Deliverables:
- Develop strategies to improve customer engagement and sales.
- Formulate goals for data mining and create a project plan.

### 2. Data Understanding
The Airbnb dataset contains information about listings, reviews, and amenities. The data understanding phase involves collecting and exploring this data to understand the key attributes that can be useful for making recommendations.

#### Key Deliverables:
- Initial data collection and description.
- Data exploration, including statistical analysis and visualizations.
- Data quality assessment and verification.

### 3. Data Preparation
In this phase, we prepare the data by cleaning and transforming it into a usable format. This includes handling missing values, selecting relevant features, and encoding amenities as binary attributes.

#### Key Deliverables:
- Data selection: Focus on listing ID, reviewer ID, amenities, and price.
- Data cleaning: Remove rows with insufficient data and handle missing values.
- Data construction: Extract amenities and create feature columns.
- Data integration: Merge multiple datasets to create a unified dataset.

### 4. Modeling
We apply several clustering algorithms to build the recommendation model. Three primary algorithms are used:
- **K-means Clustering**: Groups similar listings into clusters.
- **Agglomerative Clustering**: A hierarchical clustering approach used for creating dendrograms.
- **DBSCAN**: A density-based clustering algorithm (though this performed poorly).

#### Key Deliverables:
- Select modeling techniques and generate test data.
- Build models and assess their performance using metrics such as WCSS and dendrograms.
- Implement a recommendation system using K-means and Agglomerative Clustering.

### 5. Evaluation
The model's performance is evaluated based on business success criteria. The agglomerative clustering algorithm performed the best, grouping similar listings effectively.

#### Key Deliverables:
- Evaluate results based on business success criteria.
- Rank models and choose the best-performing one.
- Identify limitations and areas for improvement.

## Challenges and Limitations
- **Data availability**: The dataset lacked certain features that could improve classification accuracy, such as additional user preference data.
- **Feature selection**: Some features, like seasonality and price trends, influenced the model's performance, requiring careful handling during clustering.

## Next Steps
To enhance the recommendation system, the following steps are planned:
1. **Data Expansion**: Include more relevant features and datasets to improve accuracy.
2. **Model Fine-tuning**: Optimize clustering algorithms and consider additional models like GMM (Gaussian Mixture Models).
3. **Deployment**: Prepare the system for deployment and continuous evaluation in real-world scenarios.

## References
1. Chen, Yong. _Economics of Tourism and Hospitality: A Micro Approach_. Routledge, 2021.
2. "Airbnb Listings & Reviews", Kaggle, 2021. [Kaggle](https://www.kaggle.com/datasets/mysarahmadbhat/airbnb-listings-reviews).
3. CRISP-DM, IBM SPSS Modeler. [IBM Documentation](https://www.ibm.com/docs/en/spss-modeler/saas?topic=guide-introduction-crisp-dm).
