# Endpoint Behaviour Detection

Endpoint detection pipeline using **Sigma rules + ML anomaly detection** on Windows EVTX logs from attack samples.

[![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red)](https://attack.mitre.org/)
[![Sigma](https://img.shields.io/badge/Sigma-blueviolet)](https://sigmahq.io/)

## What It Does
Hybrid pipeline for EDR research:
- **Sigma rules** → Detection queries for known IOCs (LOLBins, T1218).
- **ML models** (Isolation Forest) on behavioral features: cmdline entropy, process trees, timestamps.
- Parses EVTX-ATTACK-SAMPLES for training/testing.

**MITRE Focus**: Execution (TA0002), Defense Evasion (TA0005).

## Tech Stack
- python-evtx: EVTX parsing
- sigma-py: Rule processing
- scikit-learn: Anomaly detection
- Jupyter/Pandas: Analysis

## Quick Start
```bash
git clone https://github.com/suvinmajithia/Endpoint-behaviour-detection.git
cd Endpoint-behaviour-detection
pip install evtx sigma-py scikit-learn pandas jupyter
jupyter notebook 01_threat_research.ipynb

