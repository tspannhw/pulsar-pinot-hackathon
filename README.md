# pulsar-pinot-hackathon

Apache Pulsar - Apache Pinot - Hackathon Starter

### References

* https://dev.startree.ai/docs/pinot/recipes/pulsar
* https://github.com/startreedata/pinot-recipes/tree/main/recipes/pulsar


### airquality example


#### schema.json

````
{
  "schemaName": "events",
  "dimensionFieldSpecs": [
    {
      "name": "uuid",
      "dataType": "STRING"
    }
  ],
  "metricFieldSpecs": [
    {
      "name": "count",
      "dataType": "INT"
    }
  ],
  "dateTimeFieldSpecs": [{
    "name": "ts",
    "dataType": "TIMESTAMP",
    "format" : "1:MILLISECONDS:EPOCH",
    "granularity": "1:MILLISECONDS"
  }]
}
    
````

#### table.json

````
    "stream.pulsar.bootstrap.servers": "pulsar://192.168.1.230:6650",
    
````
