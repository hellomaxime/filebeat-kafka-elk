# filebeat-kafka-elk
Filebeat Kafka Logstash Elasticsearch Kibana

---

For the example :

- __Start Kafka__
- create a kafka topic `filebeat`

- __Start Elasticsearch__
- __Start Kibana__

- Create a log file `/tmp/logs/logfile.log`

- Edit `/etc/filebeat/filebeat.yml`
- __Start Filebeat__

- __Start Logstash__
- Edit _logstash.conf_ configuration file
- `logstash -f logstash.conf --path.data /tmp/data`

- Write into `logfile.log` : `echo '[INFO] this is a test' >> logfile.log`

- Check and visualize data in __Elasticsearch__ and __Kibana__
