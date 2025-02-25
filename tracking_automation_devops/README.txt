# Tracking the Effectiveness of Automation in DevOps

## Overview
This project tracks the efficiency of DevOps automation using Prometheus and Grafana.

## Metrics Tracked:
- **Deployment Success Rate**: Percentage of successful deployments.
- **Pipeline Execution Time**: Time taken for CI/CD pipeline execution.
- **Incident Response Time**: Time taken to resolve failures.

## Setup Instructions

### 1. Install Dependencies
- Install Python 3 and required libraries:
```bash
pip install prometheus_client
```
- Install Prometheus and Grafana.

### 2. Run the Python Exporter
```bash
python automation_tracker.py
```
- This exposes automation metrics on port 8001.

### 3. Configure Prometheus
- Use the provided `prometheus.yml` file.
- Start Prometheus with:
```bash
./prometheus --config.file=prometheus.yml
```
- Access Prometheus at `http://localhost:9090`

### 4. Visualize in Grafana
- Add Prometheus as a data source in Grafana.
- Create dashboards for `deployment_success_rate`, `pipeline_execution_time`, and `incident_response_time`.

Enjoy tracking the effectiveness of automation in DevOps! 🚀
