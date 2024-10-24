# docker-opensearch-logging

A Docker-based log management setup using OpenSearch, OpenSearch Dashboard, and Logstash.

## Features
- File-based log ingestion
- Real-time log monitoring
- Full-text search
- Log visualization
- Zero configuration setup

## Requirements
- Docker
- Docker Compose

## Quick Start
```bash
# Clone repository
git clone [repo-url]
cd docker-opensearch-logging

# Create log directory
mkdir -p logs

# Add test log
echo "$(date '+%Y-%m-%d %H:%M:%S') INFO Test message" > logs/application.log

# Start services
docker-compose up -d
```

Access dashboard at: http://localhost:5601

## Log Format
```
YYYY-MM-DD HH:mm:ss LEVEL MESSAGE
```

## Services
- OpenSearch (port: 9200)
- OpenSearch Dashboard (port: 5601)
- Logstash
