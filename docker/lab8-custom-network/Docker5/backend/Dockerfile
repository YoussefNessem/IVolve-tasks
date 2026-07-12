FROM python:3.15.0b3-alpine3.24
WORKDIR /app
COPY . .
RUN pip install flask
EXPOSE 5000
CMD ["python","app.py"]