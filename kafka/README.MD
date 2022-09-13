When running on Mac M*, follow these instructions:
https://github.com/lensesio/fast-data-dev/issues/175#issuecomment-947001807

https://blog.min.io/kafka_and_minio/

---
topic: bmartins-s3-topic
bucket: bm-kafka-sink
---
kafka-topics --create --bootstrap-server localhost:9092 --topic bmartins-s3-topic
kafka-console-producer --bootstrap-server localhost:9092 --topic bmartins-s3-topic
{ "key1": "test", "message": "Hello World"}