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


#### hackathon - connect to streamnative cloud

* https://docs.pinot.apache.org/v/release-0.10.0/basics/data-import/pinot-stream-ingestion/apache-pulsar


"stream.pulsar.authenticationToken":"your-auth-token"

* https://pulsar.apache.org/docs/security-tls-keystore/


"stream.pulsar.tlsTrustCertsFilePath": "/path/to/ca.cert.pem"

