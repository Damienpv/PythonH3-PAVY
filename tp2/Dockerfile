FROM tiangolo/uvicorn-gunicorn-fastapi:python3.11-slim

COPY ./app /app

EXPOSE 80

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]
