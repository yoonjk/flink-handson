
./bin/flink run \
  -c com.demo.example.WordCount \
  /path/to/wordcount.jar \
  --input file:///data/input.txt \
  --output file:///data/output-run1