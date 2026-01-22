# Endpoint Behaviour Detection

Detects threats in Windows logs using rules + machine learning.

[![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red)](https://attack.mitre.org/)
[![Sigma](https://img.shields.io/badge/Sigma-blue)](https://sigmahq.io/)

## Overview
- Parses Windows EVTX attack samples
- Applies Sigma detection rules  
- ML finds unusual behavior patterns
- Maps to MITRE ATT&CK techniques

## Files
- `01_threat_research.ipynb` - Research notebook
- `.gitignore` - Clean repo setup

## Run It
```bash
pip install jupyter pandas scikit-learn
jupyter notebook 01_threat_research.ipynb

