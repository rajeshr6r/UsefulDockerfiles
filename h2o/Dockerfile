#h2o image
FROM  h2oai/h2o-open-source-k8s:3.34.0.3
EXPOSE 54321
CMD ["java", "-jar", "/h2o/h2o.jar"]
#python image
FROM python:3.8.13-slim-bullseye
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt
COPY . .
CMD ["python3"]
