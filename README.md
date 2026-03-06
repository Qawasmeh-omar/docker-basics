# Hello Docker (Python FastAPI) — Quick Start

This mini project shows how to run a simple **FastAPI** app inside a **Docker container**.

---

## 1) Prerequisites
- **Python 3.10+**
- **Docker Desktop** (or Docker Engine)
- (Optional) `curl` for testing

---

## 2) Project Structure
Make sure your folder looks like this:

├── app.py
├── requirements.txt
└── Dockerfile


## 3) Create a Virtual Environment (Recommended)
### Windows (PowerShell)
```bash
python -m venv .venv
.venv\Scripts\activate
```

### macOS / Linux
```python -m venv .venv
source .venv/bin/activate
```

## 4) Install Dependencies (Local Run)

``` pip install -r requirements.txt```
``` uvicorn app:app --reload```


## 4) Using Docker 

### build the docker image using: 
```docker build -t my-fastapi:1.0 .```
### Verify the image exist 

```docker images ```

### Run the Docker Container

``` docker run -p 8000:8000 my-fastapi:1.0```

### Open 

``` http://localhost:8000```