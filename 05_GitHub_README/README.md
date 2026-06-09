# Cybersecurity Risk and Incident Analytics Dashboard for SMEs

## Project Overview

This project presents a cybersecurity risk and incident analytics dashboard for a fictional small-to-medium enterprise named **RetailPro SME Ltd.** The project uses simulated cybersecurity data to analyse security incidents, vulnerabilities, business assets, risk scores, and ISO/IEC 27001 control recommendations.

The aim of the project is to convert technical cybersecurity data into management-level insights using Power BI. The dashboard helps identify common incident types, affected departments, vulnerable assets, open risks, and recommended mitigation actions.

This project combines cybersecurity, data analytics, business intelligence, and governance, risk, and compliance concepts.

---

## Business Problem

Small and medium-sized businesses often collect cybersecurity data from incidents, vulnerability scans, and risk assessments, but this information is not always presented clearly to management. Technical logs and raw security records can be difficult for non-technical decision-makers to interpret.

This project addresses the problem by creating an interactive Power BI dashboard that answers:

- What cybersecurity incidents are occurring most often?
- Which departments and systems are most affected?
- Which vulnerabilities should be patched first?
- Which business risks are highest priority?
- Which ISO/IEC 27001 controls should be prioritised?

---

## Tools and Technologies

- Power BI
- Excel
- CSV datasets
- DAX measures
- Data modelling
- Data quality validation
- ISO/IEC 27001:2022 Annex A control mapping
- Cybersecurity risk scoring

---

## Dataset

The project uses simulated SME cybersecurity data. No real company, customer, employee, or security data is used.

| Dataset | Description |
|---|---|
| Incidents | Security incident records including type, severity, department, system, status, resolution time, and business impact. |
| Vulnerabilities | Vulnerability records including CVSS score, severity, patch status, owner, and affected asset. |
| Assets | Asset inventory including asset type, department, criticality, internet-facing status, and owner. |
| Risk Register | Business risks scored using likelihood, impact, risk score, risk level, status, and department. |
| Control Mapping | ISO/IEC 27001 control mapping and recommended mitigation actions. |

---

## Data Quality Checks

Before building the dashboard, the dataset was checked for:

- Missing required values
- Duplicate IDs
- Invalid CVSS scores
- Incorrect severity classifications
- Incorrect risk score calculations
- Invalid relationships between vulnerabilities and assets
- Invalid relationships between risks and control mappings
- Inconsistent incident status and resolution time values

The final data quality audit passed all validation checks.

---

## Dashboard Pages

### 1. Executive Overview

This page provides a management-level summary of cybersecurity posture, including total incidents, high and critical incidents, open incidents, average resolution time, incident trends, severity breakdown, and affected departments.

![Executive Overview](04_Screenshots/executive_overview.png)

---

### 2. Incident Analysis

This page analyses incidents by type, severity, department, status, and resolution performance. It helps identify common incident patterns and operational response issues.

![Incident Analysis](04_Screenshots/incident_analysis.png)

---

### 3. Vulnerability and Asset Risk

This page analyses vulnerability exposure using severity, CVSS score, patch status, asset type, and internet-facing status. It supports patch prioritisation and technical remediation planning.

![Vulnerability and Asset Risk](04_Screenshots/vulnerability_asset_risk.png)

---

### 4. Risk Register and Controls

This page links cybersecurity risks to business impact, ISO/IEC 27001 controls, and recommended mitigation actions. It supports governance, risk, and compliance reporting.

![Risk Register and Controls](04_Screenshots/risk_register_controls.png)

---

## Key Insights

- Phishing, failed login attempts, and web attacks were among the most frequent simulated cybersecurity incidents.
- Finance, Sales, and IT showed higher exposure due to their use of payment, customer, and infrastructure systems.
- High and critical vulnerabilities on internet-facing assets represented the strongest remediation priority.
- Unpatched and in-progress vulnerabilities increased technical exposure.
- The highest-priority risks included phishing, account takeover, unpatched web systems, web attacks, and VPN compromise.
- Recommended controls included MFA, patch management, phishing awareness training, access control review, and incident response planning.

---

## Recommendations

| Priority | Risk Area | Recommendation |
|---|---|---|
| Critical | Account takeover | Enforce MFA across Microsoft 365, VPN, and administrator accounts. |
| Critical | Unpatched systems | Patch internet-facing high and critical vulnerabilities within seven days. |
| High | Phishing | Conduct monthly phishing simulations and targeted awareness training. |
| High | Web attacks | Apply web application firewall rules and monitor suspicious traffic. |
| High | Access control | Review CRM, HR, and finance system permissions quarterly. |
| High | Incident response | Define response SLAs and conduct incident response exercises. |
| Medium | Backup and recovery | Test backup recovery quarterly. |

---

## Skills Demonstrated

- Cybersecurity incident analysis
- Vulnerability and asset risk analysis
- Risk register development
- ISO/IEC 27001 control mapping
- Data cleaning and validation
- Power BI dashboard development
- DAX measure creation
- Data modelling and relationships
- Management-level reporting
- Business-focused cybersecurity communication

---

## Project Limitations

This project uses simulated data and should not be interpreted as a real security assessment. It does not include raw SIEM logs, endpoint telemetry, firewall events, or real vulnerability scan exports. The ISO/IEC 27001 control mapping is simplified for portfolio purposes.

---

## Future Improvements

Future improvements could include:

- Integrating real SIEM-style log data
- Adding Microsoft Defender or Wazuh-style alert records
- Adding time-based vulnerability ageing analysis
- Building automated Power Query refresh workflows
- Adding predictive or anomaly detection analysis
- Publishing the dashboard to Power BI Service
- Creating a Streamlit or web-based executive reporting portal

---

## Author

Created as a cybersecurity and business intelligence portfolio project.