# Flink Handson
## Run Flink
flink run \
  -c com.demo.example.WordCount \
  -p 1 \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar \
  --input file:///Users/nexweb/project/works/flink-handson/section-01/lab01/wc.txt \
  --output file:///Users/nexweb/project/works/flink-handson/section-01/lab01/output 

## 결과 확인
```bash
find /Users/nexweb/project/works/flink-handson/section-01/lab01/output -type f -name 'part-*' -exec cat {} +
```