UEBA Threat Detection Pipeline
Endpoint behavior analytics on Windows EVTX: ML anomaly detection + MITRE T1218 mapping

Pipeline
EVTX parsing → 250+ events

Command line extraction → 42 samples

Isolation Forest scoring → threat isolation (86% precision)

Sigma T1218 rule → LOLBin detection

MITRE ATT&CK T1218 coverage

FP/FN validation → production ready

Demo
Quickstart
bash
pip install -r requirements.txt
jupyter notebook 01_threat_research.ipynb
