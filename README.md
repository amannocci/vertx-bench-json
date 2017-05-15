## Prerequisites
* [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Maven](https://maven.apache.org/download.cgi)

## Cloning
The following steps will ensure your project is cloned properly.

1. `git clone https://github.com/amannocci/vertx-bench-json.git`
2. `cd vertx-bench-json`

## Building
To build Logbulk you simply need to run the `mvn clean package` command. You can find the compiled
JAR files in `./target` but in most cases you'll only need `benchmarks.jar`

## Running
Simply launch compiled jar :
`java -server -jar target/benchmarks.jar`

## Result
```
# Run complete. Total time: 00:27:19

Benchmark                         Mode  Cnt       Score     Error  Units
JsonBenchmark.testNewJsonArray   thrpt  200   52004,058 ± 391,153  ops/s
JsonBenchmark.testNewJsonObject  thrpt  200  103620,960 ± 681,895  ops/s
JsonBenchmark.testOldJsonArray   thrpt  200   40164,809 ± 295,782  ops/s
JsonBenchmark.testOldJsonObject  thrpt  200   78245,268 ± 608,647  ops/s
```
