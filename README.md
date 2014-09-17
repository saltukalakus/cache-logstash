ReadMe
==============
Logstash .conf files for local tests. Each sub-folder is an independent test module.


Basic
==============
A test for logstash - elasticsearch.

<b>Test setup:</b><br>
Logstash forwards nginx and ATS stat logs to elasticsearch.


Rabbitmq
==============
A test for logstash - rabbitmq - elasticsearch.

<b>Test setup:</b><br>
Logstash forwards Nginx and ATS stat logs to Rabbit-mq.
Logstash gets the logs from Rabbit-mq queue and forwards to Elasticsearch.

<b>Configurations:</b><br>
Rabbit-mq is configured in fanout (publish-subscribe) mode.