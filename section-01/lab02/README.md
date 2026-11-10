# Flink Handson
## Join
```bash
flink run \
  -c com.demo.example.join.JoinExample \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar \
  --input1 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/person \
  --input2 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/location \
  --output file:///Users/nexweb/project/works/flink-handson/section-01/lab02/joinresult 
```
## Left Outer Join
```bash
flink run \
  -c com.demo.example.join.LefOuterJoinExample \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar \
  --input1 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/person \
  --input2 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/location \
  --output file:///Users/nexweb/project/works/flink-handson/section-01/lab02/leftouter-join-result 
```

## Outer Join
```bash
flink run \
  -c com.demo.example.join.OuterJoinExample \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar \
  --input1 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/person \
  --input2 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/location \
  --output file:///Users/nexweb/project/works/flink-handson/section-01/lab02/outer-join-result 
```

## Right Join
```bash
flink run \
  -c com.demo.example.join.RightJoinExample \
  /Users/nexweb/project/works/bootcamp/wordcount/target/wordcount.jar \
  --input1 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/person \
  --input2 file:///Users/nexweb/project/works/flink-handson/section-01/lab02/location \
  --output file:///Users/nexweb/project/works/flink-handson/section-01/lab02/right-join-result 
```

 
## 결과 확인
```bash
find /Users/nexweb/project/works/flink-handson/section-01/lab02/output -type f -name 'part-*' -exec cat {} +
```