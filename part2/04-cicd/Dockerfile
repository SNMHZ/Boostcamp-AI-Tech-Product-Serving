FROM python:3.8.7-slim-buster
COPY requirements.txt ./requirements.txt
RUN pip install -r ./requirements.txt && \
    pip install 'protobuf~=3.19.0'

COPY . /app
WORKDIR /app

EXPOSE 8501
ENTRYPOINT ["streamlit", "run", "app.py", "--server.port", "8501"]



