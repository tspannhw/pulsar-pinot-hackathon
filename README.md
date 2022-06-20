# pulsar-pinot-hackathon
Apache Pulsar - Apache Pinot - Hackathon Starter



### Point to my cluster


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
