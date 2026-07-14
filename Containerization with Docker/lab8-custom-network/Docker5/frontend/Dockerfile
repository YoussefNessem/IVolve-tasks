FROM python:3.15.0b3-alpine3.24
WORKDIR /app
COPY . .
RUN pip install -r requirements.txt
EXPOSE 5000
CMD ["python","app.py"]