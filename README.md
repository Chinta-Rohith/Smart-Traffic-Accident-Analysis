# Smart Traffic Accident Analysis System

## Project Overview
The **Smart Traffic Accident Analysis System** is a Big Data Analytics and Machine Learning project designed to analyze historical road accident records, identify geographical accident patterns, and predict accident severity.

The system uses Apache Spark and PySpark to process accident data and machine learning algorithms to discover useful patterns that can support road safety analysis.

## Objectives
- Analyze historical road accident datasets.
- Identify accident severity patterns.
- Study accident frequency by time of day.
- Discover geographical accident clusters using K-Means.
- Predict accident severity using Random Forest.
- Generate analytical visualizations and insights.

## Dataset
- **Dataset:** US Accidents (March 2023)
- **Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents
- **Format:** CSV
- **Features:** Accident severity, date and time, latitude, longitude, weather conditions, temperature, humidity, visibility, wind speed, and road features.

## Technologies Used
- Python
- Apache Spark 3.5.3
- PySpark
- Spark SQL
- Spark MLlib
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- GitHub

## Machine Learning Algorithms

### 1. K-Means Clustering
K-Means clustering is used to group accident locations based on geographical coordinates (latitude and longitude).

The implementation identifies five geographical clusters to analyze accident distribution.

### 2. Random Forest Classifier
Random Forest is used to predict accident severity based on geographical, weather, and time-related features.

A weighted Random Forest model is also implemented to address class imbalance.

## Project Modules
1. Dataset Collection and Loading
2. Data Preprocessing
3. Big Data Processing Using PySpark
4. Accident Analysis Using Spark SQL
5. Geographical Hotspot Clustering
6. Accident Severity Prediction
7. Model Evaluation
8. Data Visualization

## Implementation Results
- Successfully loaded the US Accidents dataset into Apache Spark.
- Performed data preprocessing using PySpark.
- Analyzed accident severity and accident frequency by hour using Spark SQL.
- Identified five geographical clusters using K-Means.
- Trained Random Forest and weighted Random Forest classification models.
- Saved trained models to Google Drive.

### K-Means Cluster Results

| Cluster | Records |
|---|---:|
| 0 | 80,470 |
| 1 | 118,825 |
| 2 | 47,621 |
| 3 | 88,466 |
| 4 | 51,334 |

*Cluster counts represent the sampled records used during clustering.*

## How to Run
1. Open the Google Colab notebook.
2. Install the required PySpark and Python libraries.
3. Connect Google Drive.
4. Download the US Accidents dataset from Kaggle.
5. Place the CSV file in the `Traffic_Dataset` folder in Google Drive.
6. Execute the notebook cells in sequence.
7. Review the clustering results, classification evaluation, and visualizations.

## Repository Structure

```text
Smart-Traffic-Accident-Analysis/
│
├── README.md
├── Smart_Traffic_Accident_Analysis.ipynb
├── outputs/
│   ├── severity.png
│   ├── hour_analysis.png
│   └── clusters.png
│
└── models/
```

## Future Enhancements
- Real-time traffic accident data integration.
- Interactive accident hotspot maps.
- Advanced severity prediction models.
- Integration with live traffic monitoring systems.
- Improved model performance through class balancing and feature engineering.

## Conclusion
The Smart Traffic Accident Analysis System demonstrates how Big Data processing and Machine Learning can be combined to analyze historical road accident data. Apache Spark enables distributed data processing, while K-Means and Random Forest provide geographical clustering and accident severity classification capabilities.

**Developed by:** Rohith Chinta

**Project Domain:** Big Data Analytics and Machine Learning
