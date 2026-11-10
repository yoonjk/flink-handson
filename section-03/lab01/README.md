# Flink Handson
## Server 실행
```bash
nc -lk 9999
```
## Client 실행
```bash
flink run \
  -c com.demo.example.datastreamapi.WordCountStreaming \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar 
```
