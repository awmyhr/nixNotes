# ELK Stack

Versatile search and analytics tool, especially useful for use against system,
applience, and application log data.

The ELK stack is comprised of:

    - ElasticSearch [https://github.com/elastic/elasticsearch]
    - Logstash [https://github.com/elastic/logstash]
    - Kibana [https://github.com/elastic/kibana]

The entire stack is open source developed primarily by elastic[https://www.elastic.co].
It forms the core of the newer Elastic Stack (also developed by elastic), which
adds:

    - Beats [https://github.com/elastic/beats]
    - X-Pack [https://www.elastic.co/products/x-pack]
    - Cloud [https://www.elastic.co/cloud]

## Main Components

### ElasitcSearch

This is the database & search engine for the log entries and meta-data.

### Logstash

This accepts, filters, tags and processes incoming logs, then sends them to ElasitcSearch.

### Kibana

This is the front-end.

## Extras

### Beats

A data shippers for edge machines that don't have built-in ways to send data to
Logstash. This is actually a 'family' of apps.

### X-Pack 

A series of value-add plug-ins, some open/free, some not.

### Cloud

Internet-hosted portion of the product.

### Message Queuing

In the past, I have used RabbitMQ as a buffer between Logstash and ElasitcSearch.

## Architecture

The entire stack can run on a single node. I have also ran multi-node:
    
    1 viewer node (Kibana)
    1 log processor (Logstash, RabbitMQ)
    2 search nodes (ElasitcSearch control/search)
    10 data nodes (ElasitcSearch database/storage cluster)

