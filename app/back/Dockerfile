FROM python:3

COPY requirements.txt .
COPY app.py .

RUN pip install --no-cache-dir -r requirements.txt


CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]