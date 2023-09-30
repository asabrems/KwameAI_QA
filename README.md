# KwameAI_QA
---

This repository contains a Flask API application integrated with ElasticSearch, capable of processing and responding to natural language queries. 

## Quick Start

### Prerequisites

- Python 3.8.X
- Docker
- Virtual Environment (Optional but recommended)

### Steps to run the Flask API locally

1. **Clone the Repository**
    ```sh
    git clone https://github.com/your_username/flask-es-api.git
    cd flask-es-api
    ```

2. **Set up a Virtual Environment**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**
    ```sh
    pip install -r requirements.txt
    ```

4. **Set the Flask Environment Variable**
    - For Unix-based systems:
        ```sh
        export FLASK_ENV=DevelopmentConfig
        ```
    - For Windows:
        ```sh
        set FLASK_ENV=DevelopmentConfig
        ```

5. **Run the Flask API**
    ```sh
    python app.py
    ```

### Steps to run ElasticSearch using Docker

1. **Build the Docker Image**
    ```sh
    docker build -t my-elasticsearch-image . .
    ```

2. **Run the Docker Container**
    ```sh
    docker-compose up build
    ```

## API Usage

### Flask API Endpoints

- `http://localhost:5000/question`: POST request to process and respond to questions.
- `http://localhost:5000/document`: POST request to upload and index documents.

### ElasticSearch

- Accessible at `http://localhost:9200`






