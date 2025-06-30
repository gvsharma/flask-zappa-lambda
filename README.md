# flask-zappa-lambda

# Flask + Zappa + AWS Lambda

This project is a minimal Flask application deployed to AWS Lambda using [Zappa](https://github.com/Miserlou/Zappa). It also proxies vector search requests to a FAISS server running on EC2.
---

## ✅ Recommended Next Steps

### 1. 📄 Create a `README.md`

Here’s a basic starter `README.md`:

````markdown
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
````

### 2. Create a virtual environment

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### 3. Deploy to AWS using Zappa

```bash
zappa deploy dev
# or to update later:
zappa update dev
```

> Make sure to configure `zappa_settings.json` with your AWS profile, region, S3 bucket, and VPC settings.

## Endpoints

* `POST /greet` — greet a user
* `POST /vector-search` — forward request to FAISS EC2 instance

## Example Request

```bash
curl -X POST https://<your-api>/dev/vector-search \
  -H "Content-Type: application/json" \
  -d '{"query": [0.1]*16, "k": 5}'
```

## License

MIT © [GV Sharma](https://github.com/gvsharma)

````

Save that as `README.md`, commit and push:

```bash
git add README.md
git commit -m "Add project README"
git push
````

---

### 2. 📦 Add a `requirements.txt`

Run this inside your virtual environment:

```bash
pip freeze > requirements.txt
git add requirements.txt
git commit -m "Add requirements.txt"
git push
```

---

### 3. 🛡️ (Optional) Add GitHub Secrets for CI/CD (Future Step)

If you ever want to auto-deploy on push using GitHub Actions + Zappa, I can help you set that up.

---

Let me know if you want:

* A logo or badge in your README
* Help setting up GitHub Actions for auto-deploy
* Turning this into a Python package or API product

You're building something great — let’s take it all the way 💪

