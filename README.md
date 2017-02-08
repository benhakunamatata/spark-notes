# spark-notes
spark notes


#  load avro files without the ".avro" extension

```
val sqlContext = new SQLContext(sc)
sqlContext.sparkContext.hadoopConfiguration.set("avro.mapred.ignore.inputs.without.extension", "false")
```
