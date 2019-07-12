
`docker run -d --name elasticsearch --net esnet -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:6.4.3
`

**安装中文分词**

```docker exec -i -t bab86b772b05 /bin/bash

./bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v6.4.3/elasticsearch-analysis-ik-6.4.3.zip

docker restart
curl -XGET http://192.168.1.110:9200/_cat/plugins?v
```