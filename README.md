# Hummingbird Monitoring
Hummingbird monitoring using Prometheus, Grafana and Alertmanager

### Prerequistes
We need [docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) & [docker-compose](https://docs.docker.com/compose/install/) for installation.


### Prometheus configuration
Modify prometheus/prometheus.yml to update the scrape_configs for list of servers you want to monitor.
You can get more details for prometheus.yml [here](https://prometheus.io/docs/prometheus/latest/configuration/configuration/)

### Alertmanager configuration
Modify alertmanager/config.yml to add/modify different receivers/routes.
You can get more details for Alertmanager configuration [here](https://prometheus.io/docs/alerting/configuration/)

### Grafana Configuration
You can add more dashboards to Grafana UI by putting them under grafana/dashboards/. Any dashboard under this directory
will get automatically installed. By default it has a dashboard for monitoring Hummingbird.

Also you can change default grafana admin username & password by putting them under config.monitoring file.

## How to run
To run simply execute `docker-compose up -d`