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
Logstash forwards Nginx and ATS stat logs to Rabbit-mq.<br>
Logstash gets the logs from Rabbit-mq queue and forwards to Elasticsearch.<br>

<b>Configurations:</b><br>
Rabbit-mq is configured in fanout (publish-subscribe) mode.

Logprocessor
==============
A test for logstash - rabbitmq - elasticsearch - <a href="https://github.com/BATYD-Turksat/cache-log-processor">LogProcessor</a>.

<b>Test setup:</b><br>
Logstash forwards Nginx and ATS stat logs to LogProcessor over Rabbit-mq.<br>
Logstash gets processed logs of LogProcessor from Rabbit-mq queue and forwards to Elasticsearch.<br>
<br>
