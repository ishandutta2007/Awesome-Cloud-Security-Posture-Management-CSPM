# Awesome-Cloud-Security-Posture-Management-CSPM

# Awesome-Cloud-Security-Posture-Management-CSPM



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cloud Configuration Auditing, Compliance Monitoring & Security Posture*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Security Posture Management (CSPM)**. These tools help security teams continuously assess cloud configurations, detect misconfigurations, enforce compliance benchmarks, and prioritize remediation across multi-cloud environments.



**Examples** include Microsoft Defender for Cloud, Wiz, Palo Alto Prisma Cloud, Orca Security, Lacework, Datadog Cloud Security, Trend Micro Cloud One, Tenable Cloud Security, Check Point CloudGuard, and Rapid7 InsightCloudSec (the category leaders).



**Open-source emphasis**: CSPM has a **mature and production-proven open-source ecosystem**. **Prowler** and **ScoutSuite** are the two foundational defensive audit tools, both supporting AWS, Azure, and GCP with hundreds of checks mapped to compliance frameworks . **Cloud Custodian** provides a YAML-based rules engine for governance and cost optimization, while **Steampipe** enables SQL-based querying of cloud APIs without ETL . **Cloudsploit** and **ZeusCloud** offer additional open-source CSPM capabilities . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## 📖 Table of Contents



- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🤝 How to Contribute](#-how-to-contribute)

- [⚠️ Disclaimer](#-disclaimer)



## ☁️ SaaS/Hosted Platforms



> **📊 Market Context**: The global CSPM market is estimated at **~$2.5B in 2026**, growing toward **~$7B by 2031** at a **~22% CAGR**. The sector is **moderately concentrated** at the enterprise tier — Wiz, Prisma Cloud, and Microsoft Defender for Cloud form the top tier, while Orca, Lacework, and Tenable compete aggressively in the mid-market . **Pricing varies dramatically**: Microsoft Defender CSPM has a **free foundational tier** and charges only for billable workloads (VMs, storage accounts, databases) , while Prisma Cloud enterprise contracts start at **~$60K/year**  and Orca's AWS Marketplace bands run **$7,000–$30,000/month** based on concurrent EC2 workloads . **Lacework was acquired by Fortinet in 2024** for **$152.3M** and now ships as **Lacework FortiCNAPP** . No single vendor holds a winner-take-all position; enterprises typically run multi-vendor stacks.



| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |

|----------|-------------|------------------------|------------------|--------------|

| **[Microsoft Defender for Cloud](https://www.microsoft.com/en-us/security/business/cloud-security/microsoft-defender-cloud)** | **Free foundational CSPM tier** covering Azure, AWS, and GCP with secure score, security recommendations, and Microsoft Cloud Security Benchmark. **Defender CSPM** adds agentless scanning, attack path analysis, and cloud security explorer . | **Foundational CSPM**: **Free** (no time limit). **Defender CSPM**: **¥0.2/server/hour** (~$0.028/hour) for billable workloads; **¥0.096/vCore/hour** for containers . | **Free foundational CSPM** for all Azure, AWS, and GCP resources. **First 30 days free** for Defender CSPM plans; then billed per billable resource . | **~$281B revenue (Microsoft FY2025)** |

| **[Wiz](https://www.wiz.io/)** | **Agentless-first CNAPP with CSPM capabilities.** Security Graph correlates findings across compute, identity, network, data, and code. **Acquired by Google for $32B** (March 2026) after reaching **$500M revenue (2024)** and a **$12B valuation** . | **Enterprise pricing** — quote required. Typical contracts start at **~$60K/year** . | **None** — enterprise demo required. | **$32B acquisition, $500M revenue (2024), $1.9B raised**  |

| **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** | **Most feature-complete CNAPP with mature remediation engine.** 100+ compliance frameworks, agent-based runtime blocking via **Defender agents**, and **FedRAMP High + IRAP certifications** . | **Enterprise pricing** — quote required. Entry contracts start at **~$60K/year**; **the most expensive of the top three** . | **None** — enterprise demo required. | **~$9.2B revenue (Palo Alto FY2025)** |

| **[Orca Security](https://orca.security/)** | **Agentless CNAPP with SideScanning technology.** Reads cloud workload block storage out-of-band. **More competitive in mid-market** than Prisma Cloud . | **AWS Marketplace bands**: **Small $7,000/mo**, **Small-Medium $12,000/mo**, **Medium $17,000/mo**, **Large $30,000/mo** . **Typical annual contract (5,000 workloads)**: **$200K–$400K** . | **None** — no free tier or free trial publicly available . | **$1–2.5B valuation, $100–500M revenue**  |

| **[Lacework (FortiCNAPP)](https://www.lacework.com/)** | **Polygraph behavioral analytics platform.** **Acquired by Fortinet in 2024 for $152.3M**. Now ships as **Lacework FortiCNAPP** integrated into Fortinet's security fabric . | **Per-workload (agent-based)**. **Typical annual contract (5,000 workloads)**: **$150K–$350K** — lower than Orca due to agent-based architecture . | **None** — enterprise demo required. | **$152.3M acquisition (Fortinet), ~$600M raised pre-acquisition**  |

| **[Tenable Cloud Security](https://www.tenable.com/)** | **Best-in-class dedicated CIEM, now integrated into Tenable's exposure management platform.** Acquired Ermetic to add cloud identity security . | **Mid-sized deployments (500–2,500 assets)**: **$50K–$200K/year**. **Large (2,500–10,000 assets)**: **$200K–$600K/year** . | **Free trial available** — details require sales contact . | **~$900M revenue (Tenable FY2025 est.)** |

| **[Check Point CloudGuard](https://www.checkpoint.com/)** | **Unified cloud-native security with CSPM, CWPP, and network security.** **CloudGuard revenue showed weakness in CY2024** but new business grew +10% in all geographies in Q4 . | **Custom enterprise pricing** — quote required. | **30-day free trial** available. | **$2.6B revenue (Check Point FY2024)**  |

| **[Rapid7 InsightCloudSec](https://www.rapid7.com/)** | **Consumption-based CSPM with self-hosted, managed, or SaaS deployment options.** Priced on average billable resources across cloud environment . | **500 resources**: **$66,000/year**. **1,000 resources**: **$120,000/year**. **5,000 resources**: **$438,000/year**. **Developer licenses**: **$6,000/year** each . | **None** — enterprise demo required. | **~$800M revenue (Rapid7 FY2025 est.)** |

| **[Trend Micro Cloud One](https://www.trendmicro.com/)** | **Conformity module identifies 230 million misconfigurations daily** . **28% market share** in cloud workload security — **3x the second-place competitor** . | **Custom enterprise pricing** — quote required. | **Free trial available** for Conformity. | **~$1.8B revenue (Trend Micro FY2025)** |



## 🔓 Open-Source GitHub Projects



Sorted by star count (descending). Star badge links to each repo's stargazers page.



| Repo | Description | Stars |

|---|---|---|

| **[Steampipe](https://github.com/turbot/steampipe)** — **Zero-ETL cloud query engine.** Query live cloud APIs using SQL without databases. 150+ plugins covering AWS, Azure, GCP, and Kubernetes. Surface idle resources, misconfigurations, and spend patterns . AGPL-3.0. | [![Stars](https://img.shields.io/github/stars/turbot/steampipe?style=social&color=white)](https://github.com/turbot/steampipe/stargazers) | ~7,800 |

| **[Cloud Custodian](https://github.com/cloud-custodian/cloud-custodian)** — **CNCF Incubating governance engine.** YAML-based DSL for policy enforcement, off-hours scheduling, garbage collection, and utilization-based tagging. **5,959 stars** as of 2025 . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/cloud-custodian/cloud-custodian?style=social&color=white)](https://github.com/cloud-custodian/cloud-custodian/stargazers) | ~6,000 |

| **[Prowler](https://github.com/prowler-cloud/prowler)** — **Most widely used open-source CSPM.** AWS, Azure, GCP, Kubernetes, M365, GitHub, Okta with **800+ checks** mapped to CIS, NIST, PCI DSS, HIPAA, GDPR. **Lighthouse AI** for agentic cloud defense . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/prowler-cloud/prowler?style=social&color=white)](https://github.com/prowler-cloud/prowler/stargazers) | ~13,000 |

| **[ScoutSuite](https://github.com/nccgroup/ScoutSuite)** — **Multi-cloud security auditing from NCC Group.** AWS, Azure, GCP, Alibaba Cloud, OCI. Rule-based findings with severity scoring and HTML report generation . GPL-2.0. | [![Stars](https://img.shields.io/github/stars/nccgroup/ScoutSuite?style=social&color=white)](https://github.com/nccgroup/ScoutSuite/stargazers) | ~6,500 |

| **[Cloudsploit](https://github.com/aquasecurity/cloudsploit)** — **CSPM by Aqua Security.** Open-source cloud security posture management with broad cloud provider support . GPL-3.0. | [![Stars](https://img.shields.io/github/stars/aquasecurity/cloudsploit?style=social&color=white)](https://github.com/aquasecurity/cloudsploit/stargazers) | ~3,000 |

| **[ZeusCloud](https://github.com/Zeus-Labs/ZeusCloud)** — **Open-source cloud security platform.** Agentless CSPM with attack path analysis and security graph . Apache-2.0. | [![Stars](https://img.shields.io/github/stars/Zeus-Labs/ZeusCloud?style=social&color=white)](https://github.com/Zeus-Labs/ZeusCloud/stargazers) | ~600 |

| **[CloudGuard CSPM Calculator](https://github.com/CheckPointSW-Community/CloudGuard-CSPM-Calculator)** — **Check Point community tool to estimate cloud asset counts for CSPM sizing** . | [![Stars](https://img.shields.io/github/stars/CheckPointSW-Community/CloudGuard-CSPM-Calculator?style=social&color=white)](https://github.com/CheckPointSW-Community/CloudGuard-CSPM-Calculator/stargazers) | ~30 |

| **[CloudGuard CLI](https://github.com/limebrew-org/cloudguard)** — **Python CLI CSPM tool for GCP, AWS, and Azure** . | [![Stars](https://img.shields.io/github/stars/limebrew-org/cloudguard?style=social&color=white)](https://github.com/limebrew-org/cloudguard/stargazers) | ~20 |



## 🤝 How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- CSPM platforms handle sensitive cloud configuration and security data; ensure proper access controls and compliance with organizational security policies.

- **Open-source reality**: The open-source ecosystem for CSPM is **mature and production-proven** at the **defensive audit layer** (**Prowler**, **ScoutSuite**) and **governance layer** (**Cloud Custodian**, **Steampipe**) . **Prowler** is the most comprehensive open-source CSPM with 800+ checks across multi-cloud environments . However, **commercial platforms** (Wiz, Prisma Cloud, Orca, Defender for Cloud) provide **managed infrastructure, agentless scanning, attack path analysis, and enterprise support** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong cloud security engineering capacity.

- **Pricing caveat**: All pricing figures above are **verified against cited search results** but may change without notice. Enterprise contracts typically involve volume discounts, multi-year commitments, and bundled pricing . **Orca's AWS Marketplace bands** are based on **concurrent EC2 workloads** — spiky autoscaling fleets should size to peak concurrency to avoid tier jumps .



---



**Made for cloud security architects, SOC analysts, DevSecOps teams, and compliance officers.**

Let's make cloud security posture management more open, transparent, and continuously auditable.
