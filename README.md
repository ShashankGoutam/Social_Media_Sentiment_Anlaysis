# Social_Media_Sentiment_Anlaysis
Understanding real-time public sentiment on social media platforms like Reddit is essential but challenging due to the massive volume and unstructured nature of data. Traditional methods of sentiment tracking are inefficient, hence a need arises for automated tools to process and interpret trends effectively.


# 🧠 Reddit Trend Analyzer

A real-time social media analytics tool that fetches Reddit posts, analyzes public sentiment, performs topic modeling, and visualizes trending discussions using machine learning and NLP.

---

## 📌 Project Overview

Reddit Trend Analyzer is built to extract meaningful insights from Reddit discussions. It collects trending posts using the Reddit API (PRAW), stores them in MongoDB, and applies NLP techniques for cleaning, sentiment analysis, and topic modeling using LDA. KMeans clustering and data visualizations are used to highlight public opinion and discussion patterns.

---

## 🧰 Tech Stack & Tools

- **Language**: Python 3
- **APIs**: Reddit API (via `praw`)
- **Database**: MongoDB
- **NLP Libraries**: `nltk`, `TextBlob`
- **ML/Analytics**: `scikit-learn`, `LDA`, `KMeans`
- **Visualization**: `matplotlib`, `seaborn`
- **Data Handling**: `pandas`, `re`

---

## 📥 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/ShashankGoutam/Social_Media_Sentiment_Anlaysis.git
   cd reddit-trend-analyzer
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```

3. Ensure MongoDB is running locally:
   ```bash
   brew services start mongodb-community  # Mac (Homebrew)
   ```

---

## 🔧 Configuration

Create a `.env` file or set the following variables in your script:
```env
REDDIT_CLIENT_ID=your_client_id
REDDIT_CLIENT_SECRET=your_client_secret
REDDIT_USER_AGENT=RedditTrendAnalyzer/1.0
```

---

## 🚀 Usage

1. Fetch and store Reddit posts:
   ```python
   fetch_reddit_posts()
   ```

2. Preprocess and analyze:
   ```python
   df = preprocess_data()
   df = perform_sentiment_analysis(df)
   ```

3. Perform topic modeling and clustering:
   ```python
   lda_model, vectorizer = topic_modeling(df)
   df = cluster_posts(df)
   ```

4. Visualize:
   ```python
   plot_sentiment(df)
   ```

---

## 📊 Output

- Sentiment distribution histogram
- Clusters of similar discussions
- List of top extracted topics using LDA

---

## 🧪 Example Subreddits

- `r/news`
- `r/worldnews`
- `r/technology`

---

## 🧠 Future Enhancements

- Use BERT for better sentiment accuracy
- Integrate Apache Spark for big data scale
- Deploy as a web app using Streamlit or Flask

---


## 🙌 Acknowledgements

- Reddit Developers API
- Prof. Mansa K (Project Mentor)
- Libraries: TextBlob, NLTK, scikit-learn, MongoDB
