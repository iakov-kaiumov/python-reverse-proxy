# Simple reverse proxy with Python and FastAPI

A simple solution that suppors any types of requests and authorization.

## ⚡Quick Start

1. Clone this repository
    ```bash
    git clone https://github.com/iakov-kaiumov/python-reverse-proxy.git
    ```

2. Install requirements
    ```bash
   pip install -r requirements.txt
    ```
   
3. Set desired hostname in the `main.py`
    ```python
    HOSTNAME = 'hostname.com'
    ```

4. Run locally
    ```bash
    uvicorn main:app --reload --port 8000
    ```

5. Open [http://localhost:8000](http://localhost:8000)

## 🐳 Docker

1. Build the image locally:
    ```bash
    docker build --no-cache -t reverseproxy .
    ```
2. Run image:

    ```bash
    docker run -d --name flowise -p 8000:8000 reverseproxy
    ```

3. Stop image:
    ```bash
    docker stop reverseproxy
    ```
