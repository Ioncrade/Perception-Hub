# Business Sentiment Analysis 📊

A Streamlit-based web application that performs real-time sentiment analysis on news articles about companies using FinBERT. The application fetches recent news articles and provides visual insights into the sentiment distribution and trends.

## Features ✨

- Real-time news article fetching using NewsAPI
- Sentiment analysis using FinBERT (Financial domain BERT model)
- Interactive visualizations:
  - Individual sentiment distribution donut charts
  - Overall sentiment distribution
  - Sentiment scores trend over time
- User-friendly interface for company search
- Responsive design with real-time updates

## Installation 🚀

1. Clone the repository:
```bash
git clone https://github.com/yourusername/business-sentiment-analysis.git
cd business-sentiment-analysis
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file in the project root and add your NewsAPI key:
```env
NEWS_API_KEY=your_api_key_here
```

## Dependencies 📦

- streamlit
- requests
- torch
- plotly
- pandas
- transformers
- scipy
- matplotlib
- python-dotenv

## Usage 💡

1. Start the Streamlit application:
```bash
streamlit run app.py
```

2. Open your web browser and navigate to `http://localhost:8501`

3. Enter a company name in the search box and click "Analyze News"

4. View the sentiment analysis results and visualizations

## Project Structure 🏗️

```
business-sentiment-analysis/
├── app.py                  # Main application file
├── .env                    # Environment variables
├── requirements.txt        # Project dependencies
├── README.md              # Project documentation
```

## How It Works 🔄

1. **News Fetching**: The application uses NewsAPI to fetch recent news articles about the specified company.

2. **Sentiment Analysis**: Articles are analyzed using the FinBERT model, which is specifically trained for financial text sentiment analysis.

3. **Visualization**: The results are displayed through:
   - Individual donut charts for positive, negative, and neutral sentiments
   - Overall sentiment distribution
   - Interactive time series plot of sentiment scores

## API Keys 🔑

You'll need to obtain an API key from [NewsAPI](https://newsapi.org/) to fetch news articles. Once you have the key, add it to your `.env` file or Streamlit secrets.


## Analysis Example

![Screenshot 2025-01-22 183937](https://github.com/user-attachments/assets/d998557a-da07-4950-b6e8-b0491d1090d7)
![Screenshot 2025-01-22 184058](https://github.com/user-attachments/assets/fdedb9ef-9f8a-428b-a8c1-e71c92fefab6)
![Screenshot 2025-01-22 184111](https://github.com/user-attachments/assets/845edea0-047b-4932-b5d4-6bf9de342eff)


## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## License 📝

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments 🙏

- [FinBERT](https://github.com/ProsusAI/finbert) for the financial sentiment analysis model
- [NewsAPI](https://newsapi.org/) for providing news article data
- [Streamlit](https://streamlit.io/) for the web application framework
