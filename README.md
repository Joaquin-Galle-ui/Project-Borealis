<p align="center">
  <img src="assets/borealis-banner.png" alt="Project Borealis Banner" width="100%" />
</p>

<h1 align="center">Project Borealis</h1>

<p align="center">
  <strong>Enterprise Course Automation System</strong>
</p>

<p align="center">
  A private automation ecosystem built to streamline course validation, deployment, tracking, and batch processing.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Project-blue?style=for-the-badge" alt="Python Badge" />
  <img src="https://img.shields.io/badge/Automation-System-0A84FF?style=for-the-badge" alt="Automation Badge" />
  <img src="https://img.shields.io/badge/Playwright-Selenium-00C2A8?style=for-the-badge" alt="Playwright Selenium Badge" />
  <img src="https://img.shields.io/badge/SQL-Tracking-1E90FF?style=for-the-badge" alt="SQL Badge" />
  <img src="https://img.shields.io/badge/Status-Private%20Case%20Study-111827?style=for-the-badge" alt="Private Case Study Badge" />
</p>

---

## Overview

**Project Borealis** is a Python-based automation ecosystem designed to optimize and accelerate the course creation and deployment workflow.

It was built to replace repetitive, error-prone manual operations with a structured system capable of:

- validating incoming course packages
- processing large batches efficiently
- automating deployment tasks
- tracking execution state in SQL
- logging failures and preserving recoverability

Rather than being a simple script, Borealis functions as a **workflow automation system** focused on reliability, control, and operational speed.

---

## The Problem

Before Borealis, the course deployment workflow relied heavily on manual work.

This created several challenges:

- repetitive and time-consuming processing
- inconsistent data entry
- limited visibility into execution status
- difficult recovery after failed runs
- poor scalability for batch operations

In practice, large workloads could take **up to a full working week** to complete manually.

---

## The Solution

Borealis was designed to automate that workflow end-to-end.

It introduces:

- automated course validation
- state-aware deployment execution
- SQL-backed progress tracking
- duplicate prevention
- fault isolation and structured logging
- batch processing support
- a front-end interface for operational control

The result is a much faster, safer, and more scalable deployment process.

---

## Key Impact

| Metric | Result |
|--------|--------|
| Processing time reduction | **98.8%** |
| Workflow duration | **~1 week → ~20 minutes** |
| Batch throughput | **~1,000 records/hour** |
| Validation | **Automated** |
| Tracking | **SQL-backed** |
| Recovery | **Logged and resumable** |

---

## Core Features

### Automated Validation
Borealis validates incoming course packages before deployment, reducing manual review and catching issues early in the pipeline.

### Deployment Automation
The system automates key interactions required to publish and configure course content on the target platform.

### SQL State Tracking
Execution state is stored in a SQL layer, enabling visibility, safer retries, and duplicate prevention.

### Batch Processing
Borealis is designed to process large volumes of data efficiently, allowing high-throughput automation at scale.

### Fault Tolerance
Individual failures are isolated and logged, allowing the workflow to continue without collapsing the full batch.

### Operational Interface
A front-end dashboard provides visibility into uploads, deployment progress, historical processing, and execution logs.

### Secure Configuration
Sensitive data and credentials are separated through environment-based configuration and are not exposed in the repository.

---

## Workflow

```mermaid
flowchart LR
    A[Course Package Upload] --> B[Validation]
    B --> C[Data Processing]
    C --> D[Automation Engine]
    D --> E[SQL Tracking]
    E --> F[Deployment Completed]
