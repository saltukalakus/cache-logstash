logstash - rabbitmq - elasticsearch
==============
A test for logstash - rabbitmq - elasticsearch.

Test setup:
==============
Logstash forwards nginx and ATS stat logs to rabbit-mq.
Elasticsearch gets the logs from rabbit-mq queues.

Configurations:
==============
Rabbit-mq is configured in Fanout (publish-subscribe) model.


