# 🔍 OpenSearch + Dashboards (Local Dev Setup)

This project provides a local development environment using [OpenSearch](https://opensearch.org/) and OpenSearch Dashboards — an open-source search engine and visual interface similar to Elasticsearch + Kibana.

---

## ✅ Requirements

- Docker
- Docker Compose
- Node.js (if using the example client)

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

{
  "name": "opensearch",
  "cluster_name": "opensearch-cluster",
  "cluster_uuid": "...",
  "version": {
    "number": "2.14.0",
    ...
  },
  ...
}
