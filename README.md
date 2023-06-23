---
Base URL: https://flask-production-19e8.up.railway.app
Endpoint : 
  - /predict
  - /summarize
  - /topic-modeling      
---

# Project README

## Base URL: https://flask-production-19e8.up.railway.app

### Endpoint: BaseURL/predict

This endpoint allows you to submit a news article and receive predictions based on it.

- **Method:** POST
- **Description:** Submit a news article for prediction.
- **Parameters:**
  - **Input:** The news article to be predicted.
    - **Parameter:** 'news'
    - **Type:** string
    - **Example:** 'Put your news here'
    ```
    {
      "news": "Put your news here"
    }
    ```
  - **Output:** The prediction result.
    - **Type:** JSON object
    - **Example Response:**
    ```
    {
      "predict": "your response"
    }
    ```

### Endpoint: BaseURL/summarize

This endpoint allows you to submit a article and receive summarize based on it.

- **Method:** POST
- **Description:** Submit a article for summarize.
- **Parameters:**
  - **Input:** The news article to be summarized.
    - **Parameter:** 'text'
    - **Type:** string
    - **Example:** 'Put your text here'
    ```
    {
      "text": "Put your text here"
    }
    ```
  - **Input:** The news number of sentences.
    - **Parameter:** 'num_sentences'
    - **Type:** int
    - **Example:** 'Put your num_sentences here'
    ```
    {
      "num_sentences": 2
    }
    ```
  - **Output:** The summarize result.
    - **Type:** JSON object
    - **Example Response:**
    ```
    {
      "sentences": 2
      "summary": "Your summarized text" 
    }
    ```

### Endpoint: BaseURL/topic-modeling

This endpoint allows you to submit a news article and receive keywords based on it.

- **Method:** POST
- **Description:** Submit a news article for get keywords.
- **Parameters:**
  - **Input:** The news article to be shown the keywords.
    - **Parameter:** 'text'
    - **Type:** string
    - **Example:** 'Put your article or news here'
    ```
    {
      "text": "Put your news or articles here"
    }
    ```
  - **Input:** the keywords article to be shown the keywords.
    - **Parameter:** 'num_topics'
    - **Type:** int
    - **Example:** 'Put your article or news here'
    ```
    {
      "num_topics": 1
    }
    ```
  - **Output:** The keywords result.
    - **Type:** JSON object
    - **Example Response:**
    ```
    {
      "topic_keywords":
      [
        [
            "keyword",
            "keyword",
            "keyword",
            "keyword",
            "keyword"    
        ]
      ]
    }
    ```



## ✨ Features

- Python
- Flask

## 💁‍♀️ How to use

- Install Python requirements `pip install -r requirements.txt`
- Start the server for development `python3 main.py`
