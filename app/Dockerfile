FROM python:3.11-slim
WORKDIR /app
RUN pip install --no-cache-dir flask pymysql
COPY app.py .
EXPOSE 80
CMD ["python", "app.py"]

