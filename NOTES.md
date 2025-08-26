# Project notes

## Quickstart issues

- `datahub docker quickstart` seems to hung trying to connecting to a local Docker registry.
- `docker compose -f docker/quickstart/docker-compose.quickstart.yml pull` is slow but promising.
- `docker compose -f docker/quickstart/docker-compose.quickstart.yml up -d` seems to work.
- localhost:9002 works with datahub:datahub
- `datahub docker check` doesn't work.
- We add kibana service to the docker-compose file.
- Both kibana and elasticsearch are now using version 7.17.28 (M1 compatible).
- Configure Kibana index patterns to * as default (Management > Kibana > Index Patterns), next go to Discover (Analytics > Discover).
- Elasticsearch is the graph provider.
- Dejavu is better for searching in Elasticsearch. It can be accessed at http://localhost:1358
- Elasticsearch manages search and graphs: nodes for search and graphs (e.g., datasetindex_v2) and relationships between them for graphs (graph_service_v1).
