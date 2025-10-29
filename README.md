# Monitoring Stack

Personal monitoring setup for my apps using Prometheus, Grafana, and Nginx.

## Quick Start

1. Clone and run locally:
   ```bash
   git clone https://github.com/yagnikpt/app-monitoring.git
   cd app-monitoring
   docker-compose up -d
   ```

2. Access:
   - Grafana: http://localhost:3000 (admin/admin)
   - Prometheus: http://localhost:9090
   - Nginx proxy: http://localhost:5000

## Config

- `prometheus.yml`: Scrapes my personal projects every 15s.
- `nginx.conf`: Proxies Grafana and Prometheus.
- Deploy via `.github/workflows/deploy.yml` to Azure Web App.

## Notes

- Change default Grafana creds in production.
- Uses GitHub secrets for deployment.
