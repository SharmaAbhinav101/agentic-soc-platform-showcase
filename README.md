# Agentic SOC Platform Showcase

## Overview

Agentic SOC Platform is an AI-driven automated Security Operations Center (SOC) system designed to streamline cybersecurity threat detection, investigation, and response workflows.

The platform automates the complete threat analysis pipeline by ingesting endpoint security logs, normalizing log data, classifying threats using AI-inspired agents, correlating suspicious events, and generating remediation recommendations with minimal human intervention.

The project was built using a modular multi-agent architecture where specialized agents collaborate through an orchestration pipeline to reduce manual workload on security analysts and improve incident response efficiency.

The system uses:
- FastAPI for backend APIs and orchestration
- n8n for workflow automation and log ingestion
- React.js + Tailwind CSS for the SOC dashboard
- SQLite/PostgreSQL for alert and incident storage

---

# Problem Statement

Traditional Security Operations Centers (SOCs) face several challenges:
- Massive alert volumes
- High false positive rates
- Slow manual investigation
- Analyst burnout
- Delayed incident response

This project aims to solve these issues by introducing an AI-driven Agentic SOC capable of:
- Automated log ingestion
- Threat triage
- Event correlation
- Incident management
- Automated response recommendation

---

# System Workflow

```text
Endpoint Devices
      ↓
n8n Webhook Ingestion
      ↓
Log Normalization
      ↓
FastAPI Backend
      ↓
SOC Orchestrator
      ↓
Triage Agent
      ↓
Investigation Agent
      ↓
Response Agent
      ↓
Database Storage
      ↓
SOC Dashboard
