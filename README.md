# Intoxication Detection using Accelerometer and TAC (Transdermal Alcohol Concentration) Data

## Table of Contents
1. [Overview](#overview)
2. [Data Loading](#data-loading)
3. [Data Preprocessing](#data-preprocessing)
4. [Applied permutation entropy and complexity](#feature-engineering)
5. [Pattern Analysis](#pattern-analysis)
6. [Modeling](#modeling)
7. [Evaluation](#evaluation)
8. [Insights and Future Directions](#insights-and-future-directions)

## Overview <a name="overview"></a>
This project focuses on the detection of intoxication using accelerometer and TAC data collected from participants during bar crawls. The dataset was sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/515/bar+crawl+detecting+heavy+drinking). To understand the data and techniques, the research paper ["Sobriety Tracker: Detecting Heavy Drinking Episodes during Complex, Naturalistic Drinking Events"](https://killian-34.github.io/pdf/Sobriety_Tracker_IJCAI_KDH.pdf) served as a primary reference.

## Data Loading <a name="data-loading"></a>
- Utilized Python libraries to load and preprocess the dataset.
- Conducted initial exploratory data analysis to understand the structure and characteristics of the data.
- Ensured data integrity and compatibility for further analysis.

## Data Preprocessing <a name="data-preprocessing"></a>
- Converted accelerometer data from milliseconds to seconds for consistency.
- Addressed discrepancies in sampling frequency between accelerometer and TAC data.
- Segmented data based on TAC values for further analysis.

## Applied permutation entropy and complexity <a name="feature-engineering"></a>
- Applied permutation entropy and complexity analysis to detect patterns or randomness in the time series data.
- These methods were employed to extract valuable insights into the dynamics of intoxication-related signals captured by the accelerometer and TAC data.

## Modeling <a name="modeling"></a>
- Employed Random Forest classification to predict intoxication status based on accelerometer data.
- Utilized machine learning algorithms to classify participants as drunk or sober, leveraging both accelerometer and TAC data.

## Evaluation <a name="evaluation"></a>
- Assessed model performance metrics such as accuracy, precision, recall, and F1-score to evaluate the effectiveness of the classification approach.
- Identified limitations and challenges in accurately detecting intoxication solely based on accelerometer data.

## Insights and Future Directions <a name="insights-and-future-directions"></a>
- Extracted insights from the analysis, including the challenges of classifying intoxication based solely on accelerometer data.
- Proposed future research directions, such as refining classification algorithms for improved accuracy.
