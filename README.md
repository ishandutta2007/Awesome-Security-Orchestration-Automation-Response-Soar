# Awesome-Security-Orchestration-Automation-Response-Soar

## Top Security Orchestration, Automation & Response (SOAR) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Playbook Automation, Case Management & Self-Hosted SOC Workflows*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Security Orchestration, Automation & Response (SOAR)**. These tools enable SOC teams to connect disparate security systems, automate repetitive triage and response tasks, and orchestrate incident handling through playbooks—reducing mean time to respond (MTTR) and freeing analysts for higher-value work.



**Examples** include CrowdStrike Falcon Fusion, Palo Alto Cortex XSOAR, Splunk SOAR, Tines, Torq, Microsoft Sentinel Automation, Swimlane, Rapid7 InsightConnect, Sumo Logic Cloud SOAR, and D3 Security (the category leaders).



**Open-source emphasis**: SOAR is a domain where open-source tooling is **viable but requires honest acknowledgment of architectural trade-offs**. **Shuffle** is the leading dedicated open-source SOAR platform—a visual workflow editor with 200+ pre-built app integrations and access to 11,000+ endpoints via OpenAPI . **Tracecat** offers a modern Tines/Splunk SOAR alternative with Temporal-backed durable execution, YAML-as-code workflows, and free SSO/audit logs in the open-source tier . **StackStorm** provides mature event-driven automation used by Cisco, Target, and Netflix, though release frequency has declined . The critical caveat: **TheHive 5 is no longer open source**—it moved to a commercial model with a two-user Community license limit, and teams on TheHive 3/4 have no maintained upgrade path without accepting commercial terms . **n8n is not a traditional SOAR**—it lacks native case management, alert correlation, and entity behavior profiling, and should be paired with a ticketing system rather than replacing XSOAR at enterprise scale .



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon Fusion](https://www.crowdstrike.com/)**  

  SOAR and workflow automation built into the Falcon platform; orchestrates response actions across endpoint, identity, and cloud workloads with native integration to CrowdStrike telemetry.



- **[Palo Alto Cortex XSOAR](https://www.paloaltonetworks.com/)**  

  Market-leading enterprise SOAR with 1,000+ security-focused content packs, native case management, threat intelligence management (TIM), and war room collaboration. Best when paired with Palo Alto's broader security portfolio .



- **[Splunk SOAR](https://www.splunk.com/)**  

  Enterprise SOAR tightly integrated with Splunk Enterprise Security; playbook automation, case management, and a mature app ecosystem. The path of least resistance for existing Splunk ES customers .



- **[Tines](https://www.tines.com/)**  

  No-code automation platform built by former SOC practitioners; focused on simplicity and fast time-to-value for repetitive tasks and incident response workflows.



- **[Torq](https://torq.io/)**  

  AI-powered hyperautomation platform for security teams; positions itself as enterprise-grade SOAR with generative AI for workflow creation and incident triage.



- **[Microsoft Sentinel Automation](https://learn.microsoft.com/azure/sentinel/)**  

  Native automation within Microsoft Sentinel using Logic Apps playbooks; integrates with the broader Microsoft security ecosystem.



- **[Swimlane](https://swimlane.com/)**  

  Low-code security automation platform with drag-and-drop playbook builder, case management, and Turbine AI for automated triage and response.



- **[Rapid7 InsightConnect](https://www.rapid7.com/)**  

  Security automation and orchestration platform with pre-built workflows and integrations for accelerating incident response across InsightIDR and third-party tools.



- **[Sumo Logic Cloud SOAR](https://www.sumologic.com/)**  

  Cloud-native SOAR with playbook automation, case management, and integration with Sumo Logic's SIEM platform.



- **[D3 Security](https://d3security.com/)**  

  SOAR platform with visual playbook builder, case management, and threat intelligence enrichment for SOC teams.



## Open-Source GitHub Projects



### Dedicated SOAR Platforms



- **[Shuffle](https://github.com/Shuffle/Shuffle)**  

  The leading open-source **dedicated SOAR platform** built around OpenAPI, providing access to **11,000+ endpoints across 200+ pre-built app integrations** . Features: **visual workflow editor**, **app creator using OpenAPI**, premade apps for security tools, organization/sub-organization control, hybrid resource sharing with shuffler.io (optional), and a "User Input" trigger node that pauses workflow execution for analyst approval (human-in-the-loop) . **Licensing**: Shuffle itself uses AGPLv3; modular information (workflows, documentation, app SDK) uses MIT . Self-hosted via Docker Compose; cloud pricing is app-run based rather than CPU-based . **Caveats**: managing backend procedures within Docker adds complexity; integrations in containerized setups have reported reliability issues; workflow execution speed is bounded by host capacity rather than Shuffle's scheduler . **Best for SOC teams wanting a dedicated open-source SOAR with a visual editor and broad integration library**.



- **[Tracecat](https://github.com/TracecatHQ/tracecat)**  

  Open-source automation platform positioned as a **self-hosted alternative to Tines and Splunk SOAR** . Features: **workflows built via no-code drag-and-drop UI or YAML-as-code** (the two stay synchronized), workflow engine runs on **Temporal** (durable execution framework used by major cloud infrastructure teams), unlimited workflows in open-source tier, case management, built-in lookup tables, 100+ integrations, custom Python/YAML integrations with git sync, **SAML SSO, audit logs, and infrastructure-as-code deployments remain free** (unlike most commercial SOAR platforms that gate these) . Docker Compose, AWS Fargate via Terraform, and Kubernetes via Helm supported. **Caveats**: under active development with breaking changes between releases (review changelog before updating); production stack with Temporal, PostgreSQL, and optional LLMs requires infrastructure capacity; smaller community and fewer third-party integrations than older platforms . **Best for teams wanting a modern SOAR with durable execution and free SSO/audit logs**—especially those comfortable with YAML-as-code workflows.



- **[StackStorm (st2)](https://github.com/StackStorm/st2)**  

  Open-source **event-driven automation platform** used by Cisco, Target, and Netflix in production (Netflix used it for operational runbooks) . Features: rule-based automation engine, workflow management, **~160 integration packs** (NetBox, Splunk, AWS), custom scripts within workflows, and StackStorm Exchange for additional packs . **Caveats**: **no native Kubernetes support**; building and managing workflows requires **Python and YAML knowledge**; **release frequency has declined in recent years**—weigh integration breadth against operational overhead of a project with slowing community activity . Open-source version includes Slack integration; AWS integration, workflow designer, professional support, and network automation suites are **Enterprise-only** . **Best for infrastructure automation and remediation** with existing Python/YAML expertise—less suited for teams wanting a modern SOC-focused SOAR.



### Case Management & Observable Analysis (Adjacent)



- **[Cortex](https://github.com/TheHive-Project/Cortex)**  

  Open-source **observable analysis engine** (AGPL) that analyzes IPs, domains, file hashes, and emails individually or in bulk via REST API and web interface . Connects to **MISP** for threat intelligence sharing . **Critical caveat**: Cortex remains fully open-source, but **TheHive (its companion case management platform) moved to a commercial model with version 5**—after a 14-day trial, new installations require a StrangeBee license or enter read-only mode; a free Community license is available but limited to **2 users and 1 organization** . **Best for teams wanting observable enrichment**—pair with an alternative case management tool if TheHive's licensing is a barrier.



### General Automation Platforms (Not Traditional SOAR)



- **[n8n](https://github.com/n8n-io/n8n)**  

  Source-available automation platform with visual canvas and custom code; **NOT a SOAR in the traditional sense**—it lacks native case management, built-in alert correlation, and entity behavior profiling . **Honest assessment from a practitioner**: n8n workflows demonstrate SOAR *patterns* (triage, enrichment, human-approved containment) and work for a small SOC or MSSP's lightweight tier, but **a 24/7 enterprise SOC with thousands of alerts/day needs real case management, correlation, and TIM—n8n alone does not replace XSOAR, Swimlane, or Tines at that scale**. Best positioned as (a) the automation layer *around* a ticketing system that acts as the case store, or (b) a prototyping ground for playbooks later ported to a SOAR . **Security caveat**: 2026 CVE cluster and tens of thousands of unpatched, internet-exposed n8n instances—**self-hosted patching burden is not theoretical** .



### Additional Strong Open-Source Options



- **Wazuh** — Open-source SIEM/XDR (GPL-2.0) with active response capabilities; can trigger automated actions on endpoints in response to detected threats. **Not a SOAR** but provides the detection layer that feeds SOAR workflows.

- **MISP** — Open-source threat intelligence sharing platform (AGPL-3.0) with workflows supporting blocking/approval gates before event publication . **Threat intelligence layer** for SOAR enrichment.

- **TheHive 4** — **AGPL-licensed fully open source**, but no maintained upgrade path to TheHive 5 without commercial terms . Only viable for teams already running it who do not need new features.



**Frameworks for building custom systems**: For **dedicated SOAR with visual editor and broad integrations**, Shuffle provides the most complete open-source foundation . For **modern SOAR with durable Temporal execution and free SSO/audit logs**, Tracecat . For **infrastructure automation with existing Python/YAML skills**, StackStorm (accepting slowing community activity) . For **observable enrichment**, Cortex (pairing with an alternative case management tool due to TheHive 5 licensing) . **Avoid**: n8n as a XSOAR replacement at enterprise scale—it is an automation layer, not a SOAR . **TheHive 5 Community Edition** is limited to 2 users—verify licensing before adoption . No open-source platform matches Cortex XSOAR's **native case management, threat intelligence management, and war room collaboration** out of the box .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- SOAR platforms handling security credentials and incident data must comply with organizational security policies; **self-hosted SOAR tools are high-value targets**—n8n's 2026 CVE cluster and tens of thousands of exposed unpatched instances demonstrate the patching burden is real, not theoretical .

- **Open-source SOAR is viable but requires architectural honesty**—Shuffle and Tracecat provide dedicated SOAR capabilities, StackStorm provides mature automation, but **none match Cortex XSOAR's native case management, threat intelligence management, and war room collaboration** for large 24/7 SOCs . **TheHive 5 is no longer open source**—Community Edition is limited to 2 users . **n8n is not a SOAR**—it lacks case management and correlation, and should be paired with a ticketing system rather than replacing a SOAR at scale .

- Verify license terms for commercial use; Shuffle uses AGPLv3 for the core with MIT for workflows/apps , Tracecat is open-source (check repository) , and StackStorm is open-source with Enterprise-only features .



---



**Made for SOC analysts, security engineers, and teams building incident response automation.**  

Let's make SOAR more open, but with clear eyes about the case management gaps, licensing shifts, and patching burdens that define each path.
