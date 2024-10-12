# Elastic - Docker

Installation:
```
# Deploy Containers
docker compose up

# Open Docker shell & Generate service token
docker exec -it elasticsearch /bin/bash
bin/elasticsearch-service-tokens create elastic/kibana kibana-service-token-1

# OR Create a Kibana User (working)
bin/elasticsearch-users useradd kibana_user -p kibana_password -r kibana_system

# Add service token OR kibana user to .env
```

- [localhost:5601 - Kibana](http://localhost:5601)
- [localhost:5601 - ElasticSearch](http://localhost:9200)