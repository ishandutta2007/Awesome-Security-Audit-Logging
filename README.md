# Awesome-Security-Audit-Logging

## Top Security Audit Logging Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Audit Trails, Log Aggregation & Self-Hosted Compliance Logging*  

**Last updated: October 2026**



This repository tracks notable **commercial security audit logging platforms** and **open-source projects** that capture, store, and analyze audit trails for compliance, forensics, and security monitoring — from cloud-native log management to self-hosted SIEM and immutable audit storage.



**Examples** include Salesforce Audit Trail, Splunk Cloud, Datadog Cloud SIEM, Sumo Logic, LogRhythm, Papertrail, LogDNA, Mezmo, Graylog, and Logz.io (the category leaders).



**Open-source emphasis**: Security audit logging is one of the strongest open-source domains. **Wazuh** leads as the most complete open-source security platform with native audit log analysis, compliance reporting, and 4.4-star Gartner ratings . **Graylog** delivers centralized log management with an experimental MCP endpoint for LLM integration . **Security Shallots** brings a lightweight, self-hosted SIEM that runs on anything from a Raspberry Pi to a full server . **CNSL** provides correlated network security with ML anomaly detection and live dashboard capabilities . **Sentora** offers an AI-powered self-hosted SIEM, EDR, and SOAR platform with air-gap support . **Fluent Bit** and **Fluentd** handle log collection and forwarding . **Vector** provides high-performance observability data pipelines . This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Salesforce Audit Trail](https://help.salesforce.com/)**  

  **Salesforce's native audit logging** — tracks setup changes, user logins, API calls, and data access within Salesforce . **Available in Enterprise, Performance, Unlimited, and Developer editions with 30-day retention** . **Best for Salesforce customers wanting native audit trails** .



- **[Splunk Cloud](https://www.splunk.com/)**  

  **The enterprise SIEM standard with comprehensive audit logging** — mature search, correlation, and the largest app ecosystem . **Pricing scales with data volume** . **Best for large SOCs with dedicated teams** .



- **[Datadog Cloud SIEM](https://www.datadoghq.com/)**  

  **Cloud-native SIEM with audit trail monitoring** — log management, security signals, and threat detection . **Best for Datadog users wanting unified observability and security** .



- **[Sumo Logic](https://www.sumologic.com/)**  

  **Cloud-native security analytics** — automated threat detection and compliance reporting . **Best for cloud-first organizations** .



- **[LogRhythm](https://logrhythm.com/)**  

  **SIEM with native log management and SOAR** — **Best for mid-market organizations** .



- **[Papertrail](https://www.papertrail.com/)**  

  **Hosted log management** — real-time tail, search, and alerts . **Best for small teams wanting simple log aggregation** .



- **[LogDNA (Mezmo)](https://www.mezmo.com/)**  

  **Telemetry data pipeline and log analytics** — control, enrich, and route observability data . **Best for telemetry pipelines** .



- **[Mezmo](https://www.mezmo.com/)**  

  **Log management with real-time streaming** — centralized log aggregation and analysis . **Best for modern log management** .



- **[Graylog](https://www.graylog.org/)**  

  **Centralized log management** — see Open-Source section for the open-source core.



- **[Logz.io](https://logz.io/)**  

  **Cloud observability platform** — log management, metrics, and tracing on OpenSearch . **Best for unified observability** .



## Open-Source GitHub Projects



### Full SIEM & Audit Logging Platforms



- **[Wazuh](https://github.com/wazuh/wazuh)**  

  **The most complete open-source security platform with native audit log analysis**, GPLv2 licensed with **4.4-star Gartner ratings and 54+ verified reviews** . **Four components**: Indexer (OpenSearch-based), Server (log analysis engine), Dashboard (web UI), and Agent (endpoint telemetry) . **Native security log analysis, vulnerability detection, security configuration assessment, and regulatory compliance reports** — no significant third-party integration required . **Wazuh 4.14.0** added unified inventory dashboards for browser extensions, services, users, and groups . **Trade-offs**: Documentation gaps, limited active response scripts, and high resource use due to Elastic backend . **Best for comprehensive open-source SIEM with audit logging** .



- **[Security Shallots](https://pypi.org/project/security-shallots/)**  

  **Lightweight, self-hosted SIEM that runs on anything** — from Raspberry Pi to full server, no Docker required . **Ingests from Suricata, Syslog, pfSense, Wazuh, CrowdSec, Pi-hole, and Argus agents** . **Auto-detects hardware and adjusts**: Raspberry Pi (2GB) runs Suricata + syslog; Server (16GB+) runs full threat engine with baselines and ML . **Features**: alert normalization, deduplication, severity classification, pattern correlation (port scans, brute force, lateral movement), incident grouping with runbooks, and optional AI triage . **~200-400MB RAM on 4GB machine** . **Best for lightweight home labs and small SOCs needing audit logging** .



- **[Sentora](https://github.com/d3vhex/Sentora)**  

  **AI-powered self-hosted SIEM, EDR, and SOAR platform**, open-source . **Threat intel integration**: AlienVault OTX, VirusTotal, and abuse.ch feeds (Feodo, ThreatFox, URLhaus) with automatic pruning . **Air-gap mode** — all feeds and OSV mirror can be internal, nothing leaves the network . **Fleet exposure reporting** with coverage transparency . **Agent config validation** with regex compilation checking before deployment . **Best for air-gapped environments needing AI-powered security operations** .



### Log Management & Aggregation



- **[Graylog](https://github.com/Graylog2/graylog2-server)**  

  **Centralized log management with alerting and dashboards**, SSPL licensed (not OSI-approved) . **Graylog 7.0 introduced experimental Model Context Protocol (MCP) endpoint** — LLM clients can connect for natural language queries . **Four products**: Open (free), Enterprise, Security (SIEM tier), and API Security . **Trade-off**: SIEM-relevant features (anomaly detection, compliance reports) are in paid Security tier . **Best for organizations wanting polished log management UI** .



- **[Fluentd](https://github.com/fluent/fluentd)**  

  **Unified logging layer**, Apache-2.0 licensed . **500+ plugins for data collection and routing** . **The standard for log aggregation** . **Best for log collection and forwarding** .



- **[Fluent Bit](https://github.com/fluent/fluent-bit)**  

  **Lightweight log and data processor**, Apache-2.0 licensed . **The standard for Kubernetes log collection** . **4MB binary vs Fluentd's Ruby process** . **Best for edge and container log collection** .



- **[Vector](https://github.com/vectordotdev/vector)**  

  **High-performance observability data pipeline**, MPL-2.0 licensed with **18,000+ GitHub stars** . **Collect, transform, and route logs, metrics, and events** . **Rust-based for performance** . **Best for observability and log streaming** .



- **[CNSL (Correlated Network Security Layer)](https://pypi.org/project/cnsl/)**  

  **Correlated network security with ML anomaly detection**, open-source . **Features**: auth log monitoring, tcpdump network capture, GeoIP enrichment, SQLite persistence, live dashboard, 2FA, PDF compliance reports, and Grafana export . **ML anomaly detection** via scikit-learn . **Best for network-focused audit logging**.



- **[syslog-ng](https://github.com/syslog-ng/syslog-ng)**  

  **Log management with structured processing and automated archiving**, GPL-2.0 licensed . **Features**: TCP/TLS/JSON/PCRE support, log rotation and compression, and flexible filtering . **Best for syslog-based audit logging** .



### Additional Strong Open-Source Options



- **OSSEC** — Host-based intrusion detection (HIDS) that inspired Wazuh, now largely superseded .

- **Suricata** — Network IDS/IPS with deep packet inspection, not a complete SIEM but integrates with Elastic Stack .

- **OpenSearch** — Fork of Elasticsearch/Kibana with Security Analytics including Sigma rules and anomaly detection .

- **Arkime** — Large-scale packet capture and indexing for network security monitoring .

- **Elastic Stack** — Elasticsearch, Logstash, and Kibana for custom SIEM-like functionality .

- **OpenTelemetry** — Vendor-neutral instrumentation for logs, metrics, and traces .

- **Loki** — Horizontally scalable log aggregation with Grafana integration .

- **Grafana** — Visualization and dashboards for log data .



**Frameworks for building custom security audit logging solutions**: Combine **Wazuh** for comprehensive SIEM with native audit log analysis and compliance reporting . Use **Security Shallots** for lightweight, hardware-adaptive monitoring in resource-constrained environments . Deploy **Sentora** for AI-powered security operations in air-gapped environments . Choose **Graylog** for polished log management with LLM query capabilities . Integrate **Fluent Bit** or **Fluentd** for log collection and forwarding . Use **Vector** for high-performance observability data pipelines . Choose **CNSL** for network-focused audit logging with ML anomaly detection . Note that true enterprise audit logging with immutable storage, global retention policies, and vendor-supported SLAs (Splunk, Datadog, LogRhythm) remains primarily commercial territory; open-source stacks provide strong log aggregation, correlation, and compliance foundations that require integration for complete security audit logging .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Security audit logging platforms handle sensitive security telemetry and may process PII. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **Open-source audit logging has hidden costs** — engineering overhead, retention management, and compliance reporting gaps increase operational burden. A senior security engineer dedicated to log management costs more than many commercial licenses.

- **Retention requirements vary by regulation** — PCI DSS requires 1 year, HIPAA 6 years, SOX 7 years. Ensure your storage strategy meets compliance requirements .

- **License considerations**: Wazuh uses GPLv2, Graylog uses SSPL (not OSI-approved), Fluentd uses Apache-2.0, and Vector uses MPL-2.0 . Verify licensing against your use case before committing.

- The open-source ecosystem provides strong log aggregation, correlation, and compliance foundations, but **immutable storage, global retention policies, and vendor-supported SLAs** remain primarily commercial offerings.



---



**Made for security engineers, compliance officers, and organizations seeking security audit logging sovereignty.**

Let's make security audit logging more open, transparent, and compliant.
