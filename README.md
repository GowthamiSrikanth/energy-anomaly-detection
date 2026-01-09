# Energy Usage Monitoring with Context-Aware Anomaly Detection

## Overview
This project focuses on identifying unexpected energy consumption behavior by comparing actual energy usage against model-predicted expectations under normal operating conditions.

Rather than treating all anomalies as equally important, the analysis prioritizes energy behavior that cannot be explained by operational and environmental factors.

---

## Business Problem
Energy consumption naturally varies based on temperature, operating hours, and equipment condition.  
The challenge is not detecting energy spikes, but determining whether energy usage is **unexpected given the context**.

Flagging every spike leads to alert fatigue, while missing true deviations increases operational risk.

---

## Approach
- Exploratory analysis of hourly energy usage
- Baseline anomaly detection using Isolation Forest
- Identification of limitations in context-agnostic anomaly detection
- Residual-based modeling to estimate expected energy usage
- Detection of anomalies based on deviations from expected behavior
- Classification of anomalies into overload and underuse
- Priority-based interpretation for operational relevance

---

## Key Insights
- Some energy values that appeared normal visually were anomalous when evaluated contextually
- Residual-based anomalies were fewer but more meaningful
- Unexpectedly high energy usage was treated as higher operational risk
- Unexpectedly low energy usage was logged for monitoring and optimization

---

## Tools Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib  

---

## Conclusion
This project demonstrates how context-aware, residual-based analysis provides clearer and more actionable insights than surface-level anomaly detection, supporting informed and responsible decision-making.
# energy-anomaly-detection
Context-aware energy anomaly detection using residual-based modeling
