# 🔍 OpenSearch + Dashboards (Local Dev Setup)

This project provides a local development environment using [OpenSearch](https://opensearch.org/) and OpenSearch Dashboards — an open-source search engine and visual interface similar to Elasticsearch + Kibana.

---

## ✅ Requirements

- Docker
- Docker Compose

---

## 🚀 Getting Started

1. Clone this repository
2. Start the services:

```bash
docker-compose up -d
```

## 📂 Services Overview

| Service               | Port | Description                         |
|------------------------|------|-------------------------------------|
| OpenSearch             | 9200 | REST API to manage data and queries |
| OpenSearch Dashboards  | 5601 | Web interface for data exploration  |

---

## 🔌 Test the Connection

### Using cURL

```bash
curl http://localhost:9200
```

You should receive a JSON response like:

```json
{
  "name": "opensearch",
  "cluster_name": "opensearch-cluster",
  "cluster_uuid": "xyz123abc456",
  "version": {
    "number": "2.14.0",
    "build_type": "tar",
    "build_hash": "abcdef123456",
    "build_date": "2024-03-10T00:00:00Z",
    "build_snapshot": false,
    "lucene_version": "9.7.0",
    "minimum_wire_compatibility_version": "7.10.0",
    "minimum_index_compatibility_version": "7.0.0"
  },
  "tagline": "The OpenSearch Project: https://opensearch.org/"
}
```
