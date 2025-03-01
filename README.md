# Sentiment Analysis of Food Estate Merauke

## Description
This notebook contains an implementation of sentiment analysis on the topic of *Food Estate Merauke* using text processing techniques and machine learning classification. The analysis aims to understand public opinion regarding the *Food Estate* policy developed in Merauke, Indonesia.

The processes conducted in this notebook include:
1. **Data Processing**:
   - Loading a dataset of comments related to *Food Estate* obtained through YouTube scraping.
   - Shuffling the dataset to avoid bias.
   
2. **Data Preprocessing**:
   - **Text Cleaning**: Removing numbers, symbols, brackets, and emoticons.
   - **Word Normalization**: Converting informal words or abbreviations into their correct form.
   - **Stopword Removal**: Eliminating common words that do not have significant meaning in sentiment analysis.
   - **Stemming**: Reducing words to their root form using Sastrawi.

3. **Sentiment Analysis**:
   - Implementing a classification model to determine positive, negative, or neutral sentiment.
   - Evaluating model performance using specific metrics (*accuracy*, *precision*, *recall*).

---

## Sentiment Analysis Results
### Confusion Matrix and Model Evaluation
The Confusion Matrix illustrates the model's performance in classifying sentiment into three categories: **Negative (-1), Neutral (0), and Positive (1).**  
Based on the model evaluation, the following metrics were obtained:
- **Model accuracy** of **80%**, indicating the model's correctness in predicting sentiment.
- **F1-score** for each class:
  - **Negative (-1):** 0.70
  - **Neutral (0):** 0.76
  - **Positive (1):** 0.86  
  The model performs best in identifying **positive sentiment**, while **negative sentiment** has a lower recall.

### Sentiment Distribution
The *pie chart* displays the sentiment distribution of classified comments:
- **60% of comments are positive**, indicating that most users support or agree with the *Food Estate* program in Merauke.
- **22.2% of comments are neutral**, meaning they do not express a clear opinion on the policy.
- **17.8% of comments are negative**, suggesting dissatisfaction or criticism from some members of the public.

### Conclusion
- Most YouTube comments show **positive sentiment** towards *Food Estate Merauke*.
- The classification model used has a fairly good accuracy (**80%**) in classifying sentiment.
- The presence of **negative sentiment** indicates that some concerns or criticisms about the program still exist.

---

### Suggestions for Improvement:
- Further exploration of different models could help compare and optimize performance.  
- Using a larger dataset could improve model generalization.  
- Adding visualizations of sentiment analysis results could provide clearer insights into public opinion trends on *Food Estate Merauke*.  



