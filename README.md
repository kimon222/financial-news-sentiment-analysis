# Financial News Sentiment Analysis

This project uses **Natural Language Processing (NLP)** to classify financial news headlines as **bullish** or **bearish** for stock movement predictions.

![Stock Chart Gif](./assets/stock_chart.gif)

## Technologies Used:
- **NLP with VADER**: Sentiment analysis of financial headlines.
- **Python libraries**: pandas, nltk, matplotlib, scikit-learn.
  
## Details:
- I applied **VADER** (Valence Aware Dictionary and sEntiment Reasoner) to classify financial news headlines.
- The sentiment was classified into **Bullish** or **Bearish**, based on the sentiment score.

### Link to Kaggle Project:
You can view the notebook and run it directly on Kaggle:  
https://www.kaggle.com/kimonmonokandilos/financial-news-sentiment-analysis

## Getting Started

**Clone this repository**:
```bash
git clone https://github.com/yourusername/financial-news-sentiment-analysis.git
```

**Install required dependencies**:
```bash
pip3 install pandas nltk scikit-learn matplotlib
```

**Set up the VADER Lexicon**:

Download the VADER lexicon and add it to your project folder or specify the path in the script.

Run the Jupyter Notebook or Python script to see sentiment analysis in action.

**Demo**

## 📊 Sentiment Analysis Results  

**1️⃣Inputting a Financial Headline for Sentiment Analysis**  
<p align="left">
  <img src="./assets/screenshots/output1.png" alt="Financial Headline Results" width="700" height="50">
</p>  

**2️⃣Displaying the Sentiment Results of the Analysis**  
***This is before machine learning, our results from using VADER Sentiment Analysis***
<p align="left">
  <img src="./assets/screenshots/output2.png" alt="Sentiment Distribution" width="600">
</p>  

**3️⃣Visualization of the Sentiment Distribution**  
***This is after machine learning, our results from Random Forest***
<p align="left">
  <img src="./assets/screenshots/output3.png" alt="Visualization of Sentiment Distribution" width="600">
</p>  

***Explanation***:
- Top Left (TN): True Negative — The model predicted Bearish when the actual sentiment was Bearish.
- Top Right (FP): False Positive — The model predicted Bullish when the actual sentiment was Bearish.
- Bottom Left (FN): False Negative — The model predicted Bearish when the actual sentiment was Bullish.
- Bottom Right (TN): True Positive — The model predicted Bullish when the actual sentiment was Bullish.

***Random Forest Explanation***:
Random Forest can be visualized as as a team of experts (decision trees). Each expert looks at the same information (the headlines) and makes their own prediction. Then, they all come together and "vote" on the final result. This makes the prediction much more reliable than just one person's opinion (one decision tree).
