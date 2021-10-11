# kafkaintro

1. Kafka - What is - topics, partitions, replicas and offset
2. How to send. / kafka connect.
3. How to consume
4. Avro? Can we change the format?
5. Error handling, hades.
6. Command pattern

Links.
* Basic consuming https://github.com/OleBilleAtBS/kafkareceiver
* Basic sending https://github.com/OleBilleAtBS/kafkasenderservice
* Kafka admin console https://login.confluent.io/
* Kafka forum https://https://forum.confluent.io/
* Spring documentation https://docs.spring.io/spring-kafka/docs/2.8.x/reference/html/
* Hades - error handling/retry https://github.com/BESTSELLER/bestone-bi4-log-hades


Batch consuming
* The config https://github.com/BESTSELLER/bestone-bi4-log-bucket-core/blob/master/service/src/main/java/com/bestseller/bestone/bi4/log/bucket/core/service/config/KafkaConsumerConfig.java
* The listener https://github.com/BESTSELLER/bestone-bi4-log-bucket-core/blob/master/service/src/main/java/com/bestseller/bestone/bi4/log/bucket/core/service/kafkalisteners/STStyleEanListener.java


Kafka docker setup
* https://docs.confluent.io/platform/current/quickstart/ce-docker-quickstart.html?utm_medium=sem&utm_source=google&utm_campaign=ch.sem_br.brand_tp.prs_tgt.confluent-brand_mt.mbm_rgn.emea_lng.eng_dv.all_con.confluent-docker&utm_term=%2Bconfluent%20%2Bdocker&creative=&device=c&placement=&gclid=EAIaIQobChMIxPfho-bB8wIVzkaRBR3-_g8rEAAYASAAEgIpF_D_BwE

#Troubleshooting.
When creating spring boot projects and consuming from kafka. Done use devtools.
You will get classloading exceptions when consuming.

```
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-devtools</artifactId>
</dependency>
```