Microsoft Fabric Real-Time Server Telemetry & Observability Pipeline
An enterprise-grade, real-time telemetry ingestion and automated alerting pipeline built entirely within the **Microsoft Fabric** ecosystem. This project demonstrates end-to-end streaming data architecture, Kusto Query Language (KQL) analytics, and automated threshold-based alerting.

## 🚀 Business Value & Objective
Traditional IT monitoring often reacts to failures after they impact operations. This solution provides instantaneous visibility into server health metrics, streaming live telemetry data to detect anomalies, track resource utilization, and trigger automated alerts before minor spikes escalate into outages.

## 🏗️ Architecture & Data Flow
The solution leverages a modern, low-latency streaming architecture native to Microsoft Fabric:

1. **Telemetry Generation**: Simulated server metrics (CPU load, memory consumption, disk I/O, network traffic) continuously feed into the pipeline.
2. **Ingestion (Microsoft Fabric Eventstreams)**: Captures real-time streaming data securely and routes it with minimal latency.
3. **Storage & Analytics (KQL Eventhouse)**: Ingests the high-throughput stream into a Kusto database optimized for time-series telemetry data. 
4. **Real-Time Queries (KQL)**: Employs Kusto Query Language for ultra-fast aggregations, windowing functions, and anomaly detection over sliding time windows.
5. **Automated Action (Microsoft Data Activator)**: Continuously monitors the KQL query outputs to trigger automated alerts and notifications when metrics breach defined operational thresholds.
