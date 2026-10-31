# 🛡️ Awesome Security Orchestration, Automation & Response (SOAR)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> ⚡ **A curated directory of leading SaaS platforms and open-source GitHub projects for Security Orchestration, Automation, and Response (SOAR), AI-driven SOC hyperautomation, incident triage, security playbooks, and threat intelligence orchestration.**

**Security Orchestration, Automation, and Response (SOAR)** platforms empower Security Operations Center (SOC) teams, incident responders, and SecOps engineers to unify disconnected security tools, automate alert triage, orchestrate end-to-end incident containment playbooks, and dramatically reduce Mean Time to Detect (MTTD) and Mean Time to Respond (MTTR).

---

## 📑 Table of Contents

- [📊 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🏢 SaaS & Commercial Enterprise Platforms](#-saas--commercial-enterprise-platforms)
- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)
- [💡 Architectural Trade-offs & Selection Guide](#-architectural-trade-offs--selection-guide)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚖️ Disclaimer](#-disclaimer)

---

## 📊 Sector Overview & Market Dynamics

The global Security Orchestration, Automation, and Response (SOAR) market is estimated at **$1.8 billion to $2.3 billion** in 2025 and is projected to surpass **$2.6 billion by 2026**, growing at a compound annual growth rate (**CAGR**) of **14.7% to 17.4%** through 2030, propelled by exponential security alert fatigue, cybersecurity talent shortages, and strict regulatory incident disclosure mandates (e.g., SEC cyber disclosure rules and EU NIS2).

The market exhibits a **moderately concentrated top tier paired with an innovative, highly dynamic fringe**: mega-cap cloud and cybersecurity platforms (Microsoft, Palo Alto Networks, CrowdStrike, Cisco/Splunk) capture substantial enterprise suite spending through consolidated EDR/SIEM/SOAR ecosystems, while agile hyperautomation and agentic AI disruptors (Torq, Tines, Swimlane) and dedicated open-source projects capture strong standalone demand through no-code flexibility and vendor-neutral workflow orchestration.

---

## 🏢 SaaS & Commercial Enterprise Platforms

The table below summarizes leading commercial and SaaS SOAR solutions, sorted in descending order by **Company Size (Market Capitalization / Valuation / Deal Value)**:

| Platform | Company Valuation / Size | Starting Pricing | Free Tier / Free Trial Limits | Key Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Sentinel Automation](https://learn.microsoft.com/azure/sentinel/)** | **~$3.1 Trillion** (Market Cap) | **~$0.042/env hr + ~$0.00008/exec-sec** (Azure Logic Apps consumption tier) | **30-Day Free Trial** with up to $200 Azure credits; first 4,000 built-in Logic App actions free per billing month | Native Azure Logic Apps orchestration, 300+ Microsoft & 3rd-party connectors, automated incident response |
| **[Palo Alto Cortex XSOAR](https://www.paloaltonetworks.com/)** | **~$280 Billion** (Market Cap) | **~$125,000/yr** (Enterprise base tier list price via direct/EDP quotes) | **30-Day Full Trial**, then converts to permanent Community Edition capped at **166 daily automation commands**, 5 active threat feeds, & 30-day incident retention | Category-defining enterprise SOAR, 1,000+ content packs, native Threat Intelligence Management (TIM), War Room collaboration |
| **[CrowdStrike Falcon Fusion](https://www.crowdstrike.com/)** | **~$260 Billion** (Market Cap) | **$184.99/device/yr** (Included in Falcon Enterprise tier / platform bundles) | **15-Day Free Trial** of CrowdStrike Falcon platform with native Fusion SOAR workflows for up to 100 endpoints | Embedded SOAR within the Falcon platform, unified endpoint/identity/cloud telemetry, automated containment actions |
| **[Splunk SOAR](https://www.splunk.com/)** | **$28 Billion** (Acquisition Value by Cisco) | **Custom Enterprise Quote** (Workload/ingest bundled pricing; historically ~$3,000/seat/yr) | **Permanent Free Community License** (on-prem) capped at **100 licensed actions/day**, 1 tenant, and maximum 5 open cases | Deep integration with Splunk Enterprise Security, visual playbook editor, Phantom app ecosystem, case management |
| **[Sumo Logic Cloud SOAR](https://www.sumologic.com/)** | **$1.7 Billion** (Acquisition Value by Francisco Partners) | **Custom Credit Quote** (Cloud Flex Credit model, unlimited seats) | **30-Day Full-Access Free Trial** (plus a 14-day preloaded Agentic Sandbox) across Cloud SIEM & Cloud SOAR features | Cloud-native SecOps platform with automated playbook execution, alert triage, and incident lifecycle management |
| **[Torq](https://torq.io/)** | **$1.2 Billion** (Valuation, 2026 Series D) | **Custom Quote** (Torq Essential vs. Pro SOC tiers, multi-agent pricing) | **No Public Free Tier**; evaluation via scheduled guided sales demo and coordinated 14-to-30 day POC sandbox | AI-native SOC hyperautomation, autonomous multi-agent playbooks, natural language workflow creation |
| **[Tines](https://www.tines.com/)** | **$1.125 Billion** (Valuation, 2025 Series C) | **$500/month** (~$6,000/yr billed annually for Starter/Core self-serve plans) | **Forever Free Community Edition**: 1 builder seat, **3 active stories/workflows**, unlimited view-only users, and core integrations | No-code workflow automation engineered for SecOps practitioners, durable execution, instant API connectors |
| **[Rapid7 InsightConnect](https://www.rapid7.com/)** | **~$1.0 Billion** (Market Cap) | **Custom Job-Tier Quote** (Priced on automation job volume or bundled with InsightIDR) | **30-Day Free Trial** across Rapid7 Insight platform with active orchestration modules upon sales request | 300+ pre-built security plugins, cross-product automation with InsightIDR and InsightVM, automated containment |
| **[Swimlane](https://swimlane.com/)** | **>$300 Million** (Growth Capital Raised) | **Custom Action-Tier Quote** (Turbine Starter through Elite tiers, unlimited users/playbooks) | **No Public Self-Service Tier**; 30-day proof-of-concept (POC) sandbox arranged via enterprise sales | Low-code security automation, Turbine Canvas workflow engine, Hero AI autonomous triage assistant |
| **[D3 Security](https://d3security.com/)** | **~$15 Million** (Total Funding; ~$25M-$50M Est. Revenue) | **Custom Alert-Tier Quote** (Subscription tiered by 500 to 10,000+ daily alerts + named seats) | **No Public Free Tier**; proof-of-concept trial arranged via sales demonstration and threat scenario scoping | D3 Smart SOAR and Morpheus AI, fixed daily alert volume model, MITRE ATT&CK auto-correlation, multi-tenant MSSP support |

---

## 🔓 Open-Source GitHub Projects

The table below lists top open-source projects for SOAR, security automation, case management, and threat intelligence, ranked in descending order by **GitHub Stars**:

| Project | Stars | Primary Focus & Architecture | License |
| :--- | :--- | :--- | :--- |
| **[n8n](https://github.com/n8n-io/n8n)** | [![GitHub stars](https://img.shields.io/github/stars/n8n-io/n8n?style=social&color=white)](https://github.com/n8n-io/n8n/stargazers) | **General Workflow Automation**: Visual node-based workflow engine with 400+ nodes and webhook triggers. *Note: Not a dedicated SOAR; lacks native case management and entity correlation, but widely deployed as a lightweight SOC automation pipeline.* | Sustainable Use License (Fair-code) |
| **[Wazuh](https://github.com/wazuh/wazuh)** | [![GitHub stars](https://img.shields.io/github/stars/wazuh/wazuh?style=social&color=white)](https://github.com/wazuh/wazuh/stargazers) | **SIEM / XDR Active Response**: Unified agent for threat detection and compliance with built-in Active Response scripts to drop malicious connections, isolate hosts, and block brute-force attacks. | GPL-2.0 |
| **[MISP](https://github.com/MISP/MISP)** | [![GitHub stars](https://img.shields.io/github/stars/MISP/MISP?style=social&color=white)](https://github.com/MISP/MISP/stargazers) | **Threat Intelligence Orchestration**: Open-source threat intelligence sharing platform with automated IOC synchronization, sharing communities, and automated enrichment feeds. | AGPL-3.0 |
| **[StackStorm (st2)](https://github.com/StackStorm/st2)** | [![GitHub stars](https://img.shields.io/github/stars/StackStorm/st2?style=social&color=white)](https://github.com/StackStorm/st2/stargazers) | **Event-Driven Automation Engine**: Mature rule-based automation engine with ~160 integration packs, Orquesta workflow runner, and automated infrastructure remediation. | Apache-2.0 |
| **[Netflix Dispatch](https://github.com/Netflix/dispatch)** | [![GitHub stars](https://img.shields.io/github/stars/Netflix/dispatch?style=social&color=white)](https://github.com/Netflix/dispatch/stargazers) | **Security Incident Management**: All-in-one crisis and incident orchestration platform developed by Netflix to manage Slack/Zoom war rooms, track incident lifecycle, and assign action items. | Apache-2.0 |
| **[TheHive](https://github.com/TheHive-Project/TheHive)** | [![GitHub stars](https://img.shields.io/github/stars/TheHive-Project/TheHive?style=social&color=white)](https://github.com/TheHive-Project/TheHive/stargazers) | **Security Incident Response (SIRP)**: SOC case management platform with real-time collaboration, dynamic task checklists, and MISP synchronization. *(v4 AGPL-3.0; v5 StrangeBee commercial model with 2-user Community edition).* | AGPL-3.0 / Commercial |
| **[Tracecat](https://github.com/TracecatHQ/tracecat)** | [![GitHub stars](https://img.shields.io/github/stars/TracecatHQ/tracecat?style=social&color=white)](https://github.com/TracecatHQ/tracecat/stargazers) | **AI-Native Dedicated SOAR**: Modern self-hosted SOAR powered by Temporal durable workflow execution, YAML-as-code and visual drag-and-drop builders, incident triage, and built-in case management. | AGPL-3.0 / Apache-2.0 |
| **[Shuffle](https://github.com/Shuffle/Shuffle)** | [![GitHub stars](https://img.shields.io/github/stars/Shuffle/Shuffle?style=social&color=white)](https://github.com/Shuffle/Shuffle/stargazers) | **Dedicated Open-Source SOAR**: Premier open-source SOAR platform featuring an interactive visual canvas, OpenAPI app generator connecting to 11,000+ endpoints, human-in-the-loop approval nodes, and Docker execution. | AGPL-3.0 |
| **[FIR (Fast Incident Response)](https://github.com/certsocietegenerale/FIR)** | [![GitHub stars](https://img.shields.io/github/stars/certsocietegenerale/FIR?style=social&color=white)](https://github.com/certsocietegenerale/FIR/stargazers) | **Cybersecurity Incident Tracker**: Lightweight CERT incident response case tracker created by Société Générale for tracking compromised assets, business lines, and IOC statistics. | AGPL-3.0 |
| **[Cortex](https://github.com/TheHive-Project/Cortex)** | [![GitHub stars](https://img.shields.io/github/stars/TheHive-Project/Cortex?style=social&color=white)](https://github.com/TheHive-Project/Cortex/stargazers) | **Observable Analysis Engine**: Automated observable triage and active response engine that analyzes IPs, hashes, URLs, and domains via 100+ analyzers and responders over REST APIs. | AGPL-3.0 |
| **[DFIR-IRIS](https://github.com/dfir-iris/iris-web)** | [![GitHub stars](https://img.shields.io/github/stars/dfir-iris/iris-web?style=social&color=white)](https://github.com/dfir-iris/iris-web/stargazers) | **Collaborative IR Platform**: Web-based incident response platform designed for SOC/DFIR teams to organize investigations, graph evidence, parse forensic timelines, and share indicators. | LGPL-3.0 |
| **[Demisto Content](https://github.com/demisto/content)** | [![GitHub stars](https://img.shields.io/github/stars/demisto/content?style=social&color=white)](https://github.com/demisto/content/stargazers) | **Open SOAR Playbook Repository**: Official open-source community repository for Palo Alto Cortex XSOAR integrations, incident playbooks, automation scripts, and detection rules. | MIT |
| **[CISA Shareable SOAR Workflows](https://github.com/cisagov/shareable-soar-workflows)** | [![GitHub stars](https://img.shields.io/github/stars/cisagov/shareable-soar-workflows?style=social&color=white)](https://github.com/cisagov/shareable-soar-workflows/stargazers) | **Standardized SOAR Playbooks**: Open-source, vendor-neutral automated security workflows published by CISA mapped to the NIST Cybersecurity Framework in BPMN format. | CC0-1.0 |
| **[DeepAlert](https://github.com/cookpad/deepalert)** | [![GitHub stars](https://img.shields.io/github/stars/cookpad/deepalert?style=social&color=white)](https://github.com/cookpad/deepalert/stargazers) | **Serverless Cloud SOAR**: Serverless security automation framework built with AWS Lambda and CDK that automatically correlates, assesses, and responds to cloud security findings. | Apache-2.0 |

---

## 💡 Architectural Trade-offs & Selection Guide

When designing an automated Security Operations pipeline, engineering teams must balance **commercial convenience vs. open-source control**:

```
                       What is your SOC team's primary automation requirement?
                                                │
         ┌──────────────────────────────────────┼──────────────────────────────────────┐
         │                                      │                                      │
   Enterprise SOAR                     Dedicated Open-Source                    Custom Automation
         │                                      │                                      │
  Need native TIM, War                   Visual editor & full                  Lightweight pipelines,
  Rooms, and 24/7 support?              self-hosted control?                    internal scripting?
         │                                      │                                      │
  [Cortex XSOAR / Splunk SOAR /          [Shuffle / Tracecat]                  [n8n + TheHive /
   Swimlane / Tines / Torq]                                                     StackStorm / Cortex]
```

### 1. Dedicated Open-Source SOAR Platforms
* **[Shuffle](https://github.com/Shuffle/Shuffle)** is the gold standard for teams requiring a dedicated visual drag-and-drop SOAR with an extensive OpenAPI connector catalog (11,000+ endpoints) and built-in human-in-the-loop analyst gates.
* **[Tracecat](https://github.com/TracecatHQ/tracecat)** provides an agile, code-centric alternative built on Temporal durable execution, making workflows resilient against network dropouts with bidirectional YAML/UI sync and free SAML SSO.

### 2. General-Purpose Automation vs. True SOAR
* **[n8n](https://github.com/n8n-io/n8n)** has become an immensely popular automation backbone, but **is not a native SOAR**: it lacks built-in case management, security entity correlation, and threat intelligence deduplication. For production SOCs, pair n8n with dedicated case management like **[DFIR-IRIS](https://github.com/dfir-iris/iris-web)** or **[TheHive](https://github.com/TheHive-Project/TheHive)**.

### 3. Case Management & Analysis Infrastructure
* For incident investigation and forensic evidence tracking, deploy **[DFIR-IRIS](https://github.com/dfir-iris/iris-web)** or **[TheHive](https://github.com/TheHive-Project/TheHive)**.
* For automated IOC enrichment (IPs, hashes, domain reputation), hook your playbooks into **[Cortex](https://github.com/TheHive-Project/Cortex)** and **[MISP](https://github.com/MISP/MISP)**.

---

## 🤝 How to Contribute

Contributions are welcome! Please follow these steps:

1. 🍴 **Fork the repository** on GitHub.
2. 🔍 **Verify details**: Ensure open-source projects include a valid repository link, star badge, active maintenance status, and open license. Ensure commercial entries include specific starting tiers and verifiable free trial parameters.
3. 📝 **Preserve table schemas**: Maintain tabular formatting, markdown links, and sorting criteria.
4. 🚀 **Submit a Pull Request** with a concise description of the addition.

---

## ⚖️ Disclaimer

- This repository is a community-curated list for educational and research purposes and does not constitute commercial endorsement.
- Running self-hosted security automation engines handling API keys, cloud tokens, and incident logs requires strict network isolation, secrets vaulting, and continuous vulnerability patching.
- All product names, logos, and trademarks belong to their respective holders.
