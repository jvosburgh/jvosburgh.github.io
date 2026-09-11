---
title: Jason Vosburgh Technical Explaner for the GoVAC® System Cloud-Based SCADA Data Flows
layout: default
---
# How Operational Data Is Ingested, Processed, Visualized, and Used by Utility Operators & ESG Teams

## Overview
Pipeline evacuation and gas-capture operations generate large volumes of telemetry: pressures, temperatures, flow rates, engine performance, and environmental metrics. The GoVAC® IloT Reporting System transforms this raw field data into structured, actionable intelligence through a cloud-based SCADA workflow. Utility operators use this data to manage operations in real time, while ESG teams rely on it for emissions accounting, regulatory reporting, and methane-reduction verification.

This explainer outlines how operational data moves from field equipment to cloud-based dashboards and environmental impact reports.

---

## 1. Data Ingestion — Secure Capture From Field Equipment
Each GoVAC unit streams operational data through an onboard cellular modem/gateway. This gateway establishes a secure, encrypted connection to the cloud and continuously transmits:

- Multi-stage inlet/outlet pressures  
- Temperature readings across compressor stages  
- Flow rates (SCFM, lbs/hr, totalized flow)  
- Engine RPM, load, battery voltage  
- System mode states and alarms  
- Environmental attributes (fuel consumption, emissions factors)

This ingestion layer ensures that all field data is captured directly from sensors and control systems, eliminating manual transcription and reducing error.

---

## 2. Data Processing — Normalization, Tag Mapping & Time-Series Structuring
Once ingested, the SCADA backend processes the data through several steps:

### Tag Normalization
Sensor values (PT01–PT13, TE02–TE14, FT01–FT02, etc.) are mapped to standardized tag definitions so operators and ESG teams see consistent naming across all units.

### Time-Series Structuring
All telemetry is timestamped, sequenced, and stored as time-series data. This enables:

- Trend analysis  
- Multi-unit comparisons  
- Project-level reporting  
- Historical playback  

### Derived Calculations
The system computes additional metrics such as:

- Total natural gas evacuated  
- Compressor efficiency  
- Fuel consumption  
- Emissions from operations  
- Net natural gas recovered (MT CO₂e)

These derived values feed directly into environmental impact reporting.

---

## 3. Data Visualization — Real-Time Dashboards & Live P&ID
The processed data is visualized through a browser-based SCADA dashboard.

### Fleet Overview
Operators see:

- Online/offline status  
- Run hours  
- Inlet/outlet pressures  
- Flow totals  
- System mode states  

### Unit Detail Pages
Each unit provides a full telemetry view with:

- Real-time pressure and temperature charts  
- Flow rate graphs  
- Engine performance metrics  
- Alarm and event logs  

### Live P&ID
A dynamic P&ID diagram displays real-time values mapped to each sensor tag, giving operators an intuitive, spatial understanding of system behavior.

### Trend Analysis
Operators can generate:

- Quick trends (pressure, temperature, flow, power)  
- High-resolution ad-hoc trends  
- Multi-unit comparisons  

This supports both operational decision-making and post-project analysis.

---

## 4. Operational Use — Real-Time Decision Support
Utility operators use the SCADA data to:

- Monitor pipeline evacuation progress  
- Validate compressor performance  
- Detect anomalies or unsafe conditions  
- Optimize evacuation speed and efficiency  
- Coordinate field crews and maintenance  
- Ensure compliance with operating procedures  

Real-time visibility reduces downtime, improves safety, and increases gas-recovery efficiency.

---

## 5. ESG Use — Emissions Accounting & Regulatory Reporting
ESG teams rely on the processed data for:

### Emissions Quantification
The system calculates:

- Methane captured  
- Methane avoided  
- CO₂e reductions  
- GoVAC operational emissions  
- Net environmental benefit  

### Regulatory Compliance
Data supports:

- State and federal reporting  
- Methane-reduction programs  
- Utility emissions disclosures  
- Pipeline maintenance documentation  

### Audit-Ready Records
Because all data is measurement-based and cryptographically secured, ESG teams receive:

- Immutable chain-of-custody  
- Digitally notarized emissions calculations  
- Verifiable project-level environmental impact reports  

This ensures transparency and credibility for internal ESG reporting, investor disclosures, and regulatory filings.

---

## Why This Matters
By digitizing the entire operational workflow, the GoVAC IloT Reporting System gives utilities and ESG teams a unified, trustworthy source of truth. Operators gain real-time situational awareness, while ESG teams receive defensible, measurement-based emissions data — enabling cleaner operations, stronger compliance, and credible methane-reduction reporting.

