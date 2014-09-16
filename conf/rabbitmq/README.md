Logstash - Rabbitmq - Elasticsearch
==============
A test for logstash - rabbitmq - elasticsearch.

Test setup:
==============
Logstash forwards Nginx and ATS stat logs to Rabbit-mq.
Elasticsearch gets the logs from Rabbit-mq queues.

Configurations:
==============
Rabbit-mq is configured in fanout (publish-subscribe) mode.

Elasticsearch gets data from Rabbit-mq with <a href="https://github.com/elasticsearch/elasticsearch-river-rabbitmq">elasticsearch-river-rabbitmq</a> plugin.

