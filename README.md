# Hotel Review Sentiment Analysis for Customer Insights

## Introduction

Social media and online reviews are crucial in shaping customer decisions and business reputation in the hospitality industry. This project analyzes hotel reviews from social platforms to uncover patterns in sentiment, ratings, and preferences, providing insights into customer satisfaction across different locations and time periods.

## Data Overview

The dataset contains:

- **Hotel Information**: Name, address, city, country, coordinates (latitude and longitude), postal code, province.
- **Review Details**: Ratings (0-5 scale), review text, recommendation status.
- **Reviewer Information**: Username, user city, user province, review dates.

## Business Understanding

The goal of this project is to analyze hotel reviews to identify customer satisfaction trends and preferences. Insights from ratings and sentiment analysis help hotels enhance services and maintain competitiveness.

## Key Questions

1. **What is the distribution of ratings?**
2. **How do reviews vary across different locations?**
3. **What themes are common in positive and negative reviews?**
4. **How do sentiments correlate with ratings?**

## Methodology

### Data Preprocessing

- **Missing Values**: Checked for missing data and addressed it by dropping or filling missing values.
- **Data Cleaning**: Cleaned the review texts by converting to lowercase, removing punctuation, and eliminating stopwords using NLTK.
- **Feature Engineering**: Created a binary sentiment label based on ratings (positive if rating ≥ 4, negative otherwise).

### Exploratory Data Analysis (EDA)

- **Rating Distribution**: Analyzed the distribution of ratings to understand overall customer satisfaction.
- **Location Analysis**: Identified top cities and provinces by the number of reviews and average ratings.
- **Hosting Names**: Determined the most and least popular hotels based on the number of stays.
- **Visualizations**: Used bar plots and heatmaps to visualize findings.

### Sentiment Analysis

- **Text Vectorization**: Converted textual data into numerical data using TF-IDF Vectorization.
- **Model Training**: Split the data into training and testing sets and trained a Logistic Regression model to predict sentiment.
- **Evaluation**: Assessed model performance using a classification report and confusion matrix.
- **Word Clouds**: Generated word clouds for overall, positive, and negative reviews to identify common themes.

## Results

- **Model Performance**: The Logistic Regression model achieved an accuracy of approximately 81%, indicating good performance in predicting sentiment from review text.
- **Common Themes**:
  - *Positive Reviews*: Words like "clean", "friendly", "comfortable", and "excellent" were prevalent.
  - *Negative Reviews*: Frequent mentions of "dirty", "noisy", "poor", and "disappointing".
- **Location Insights**:
  - *Highest Ratings*: California (CA) and New York (NY) had the highest average ratings, suggesting higher customer satisfaction.
  - *Areas for Improvement*: Some provinces showed lower ratings, highlighting regions where service enhancements are needed.

## Conclusion

The sentiment analysis revealed that 75% of the reviews were positive, with cleanliness and service quality being significant factors for customer satisfaction. To improve, hotels should focus on enhancing service quality in lower-rated areas and leverage positive feedback in marketing strategies. Addressing common complaints, particularly in customer service, can significantly reduce negative reviews.

**Recommendations**:

- **Service Improvement**: Enhance training programs for staff in lower-performing locations.
- **Feedback Utilization**: Use positive reviews in promotional materials to attract more customers.
- **Complaint Resolution**: Implement efficient mechanisms to address and resolve customer complaints promptly.
- **Future Work**: Integrate real-time sentiment tracking and conduct competitor analysis for deeper insights.

## Dependencies

- **Python Libraries**:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - nltk
  - scikit-learn
  - wordcloud

## How to Run

1. **Install Required Packages**:

   ```bash
   pip install pandas numpy matplotlib seaborn nltk scikit-learn wordcloud
   ```

2. **Download Dataset**:

   - Ensure the `Hotel_data.csv` dataset is in your working directory.

3. **Run the Script**:

   - Execute the Python script or Jupyter notebook containing the analysis.

4. **NLTK Data Download**:

   - In the script, ensure you download the necessary NLTK data packages:

     ```python
     import nltk
     nltk.download('stopwords')
     nltk.download('punkt')
     ```

## Acknowledgments

- **Data Source**: The dataset was sourced from social media and online review platforms relevant to the hospitality industry.
- **Libraries Used**:
  - Data manipulation and analysis: pandas, numpy
  - Data visualization: matplotlib, seaborn
  - Natural Language Processing: nltk
  - Machine Learning: scikit-learn
  - Word Cloud Generation: wordcloud

## Contact Information

For any questions or further information, please contact:

- **Name**: [Mohammed Alqarni]
- **Email**: [M30.alqarni@gmail.com]

