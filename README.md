## Using Prometheus and Grafana To visualize host and containers metrics
Using Prometheus and Grafana to monitor Metrics

**Setup**  
Run the below commands to download and Prometheus and Grafana.  
```bash
#Downloading the repository
git clone git@github.com:hiepdng/prometheus_grafana_metrics.git

#Creating volumes
cd prometheus_grafana_metrics
mkdir prometheus_data
sudo chown -R nobody:nogroup prometheus_data
mkdir grafana_data
sudo chown -R 472:472 grafana_data

#Running containers
docker compose up -d
```
**Access Grafana web:**  
Go to http://localhost:3000/ to access your local Grafana webpage and view the host and containers metrics.  

To view specific container webpages:  
- Prometheus: http://localhost:9090/
- Node-exporter: http://localhost:9100/

