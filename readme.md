# Elastic Playground

The ElasticStack is the perfect tool for understanding exception
management, application health, and usage patterns. By using your
application logs and some minor transformation you can ship searchable,
scalable monitoring infrastructure.

## Setup

This Elastic Stack demo runs super easily assuming you have Docker
installed. I'd recommend referring to the [official install
guide](https://docs.docker.com/compose/install/) for details on getting
up and running.

From there `docker-compose up` will spin up:

1. A simple [express.js](https://expressjs.com/) app with a
   [Logstash](https://www.elastic.co/logstash) adapter to send
application logs to Elasticsearch.
2. [Elasticsearch document
   database](https://www.elastic.co/elasticsearch/) to store application
logs
3. [Kibana](https://www.elastic.co/kibana/) visualization service

## Fake Traffic Generator

by running `npm run fake-traffic` a fake steady stream of data will be
sent to the express app for you to visualize and interact with.
