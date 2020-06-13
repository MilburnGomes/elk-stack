# elk-stack
Elasticsearch Logstash Kibana (ELK) Stack

To run elasticsearch. Go to the bin folder of elasticsearch and then type elasticsearch, as shown below:
```
cd D:\2020\Logstash\elasticsearch-7.7.1-windows-x86_64\elasticsearch-7.7.1\bin
D:\2020\Logstash\elasticsearch-7.7.1-windows-x86_64\elasticsearch-7.7.1\bin>elasticsearch
```

To run kibana. Go to the bin folder of kibana and then type kibana, as shown below:
```
cd D:\2020\Logstash\kibana-7.7.1-windows-x86_64\kibana-7.7.1-windows-x86_64\bin
D:\2020\Logstash\kibana-7.7.1-windows-x86_64\kibana-7.7.1-windows-x86_64\bin>kibana
```

To run logstash . Go to the bin folder of logstash and then type logstash followed by `-f` and the config file path with name, as shown below:

```
cd D:\2020\Logstash\logstash-7.7.1\logstash-7.7.1\bin
D:\2020\Logstash\logstash-7.7.1\logstash-7.7.1\bin>logstash -f "D:\2020\Logstash\data\logstash_movies.config"
```


Kibana Dev Tools:
movies get all endpoint:
```
GET /movies
```


movies search endpoint:
```
GET /movies/_search
{
  "query": {
    "match_all": {}
  }
}
```

movies count endpoint:
```
GET /movies/_count
```
