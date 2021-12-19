# Secure_Coding
Search_Engine Secure Coding round Final

# Introduction 
This project all about creating robust  search engine , It's  secure reason behind i am using django framework (basicaly django prevent xss csrf ) ,for robust search and giving great result i use ElasticSearch.

# Why ElasticSearch:
Elasticsearch is a search engine based on the Lucene library. It provides a distributed, multitenant-capable full-text search engine with an HTTP web interface and schema-free JSON documents


# Technology:
1. ElasticSearch 7.16.1
2. Django  version 3.2


# Setup
## Run a ElasticSearch on Docker:
```
docker pull docker.elastic.co/elasticsearch/elasticsearch:7.16.1
```
## Start a elastic 
```
docker run -p 127.0.0.1:9200:9200 -p 127.0.0.1:9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.16.1
```

# Start a virtual environment
```
virtualenv venv
```

# Initialize the virtualenv
```
source venv/bin/activate
```
## If powershell
```
powershell.exe -ep bypass
.\venv\Scripts\activate.ps1
```

# Install the requirements
```
pip3 install -r req.txt
```

# Sending Data to Elastic Search:
```
python3 upload.py
```
# Run the server
```
python3 .\searchengine\manage.py runserver
```
