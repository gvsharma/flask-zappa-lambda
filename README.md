# flask-zappa-lambda

# Flask + Zappa + AWS Lambda

This project is a minimal Flask application deployed to AWS Lambda using [Zappa](https://github.com/Miserlou/Zappa). It also proxies vector search requests to a FAISS server running on EC2.

## Features

- 🐍 Python + Flask REST API
- 🚀 Serverless deployment with Zappa
- 🔍 `/vector-search` endpoint for FAISS similarity search
- 🧠 `/greet` sample route

## Getting Started

### 1. Clone this repo

```bash
git clone https://github.com/gvsharma/flask-zappa-lambda.git
cd flask-zappa-lambda
