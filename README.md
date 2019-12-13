# aws-nlb-s3-es
Push NLB logs from S3 to AWS Elasticsearch using Lambda.

Introduction

This example solves a specific use case where logs from AWS NLB which are stored in an S3 bucket needs to be streamed to AWS ElasticSearch service for analysis and visualization. NLB logs can be configured to be stored into an S3 bucket from where a lambda can be triggered to stream logs to ElasticSearch service. The lambda code (in Python) parses the NLB logs (in S3) and converts each line into JSON so that visualizations in Kibana can be easily configured. 

The Python code also uses <> so that the location of incoming Public IPs are mapped to the respective Country and City of origin. You may want to keep this customization or remove it as per your use-case.

