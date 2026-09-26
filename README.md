# Awesome-Attack-Surface-Management

# Top Attack Surface Management (ASM) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on External Asset Discovery, Continuous Exposure Monitoring, Subdomain & Service Enumeration, and EASM Intelligence*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Attack Surface Management (ASM / EASM)**. These systems discover and monitor internet-facing assets—domains, IPs, cloud resources, APIs—so security teams can reduce unknown exposure and prioritize remediation.

**Examples** include Wiz, UpGuard, Rapid7, Recorded Future Attack Surface Intelligence, Assetnote, Detectify, ProjectDiscovery Cloud, Censys, NetSPI, Bishop Fox Cosmos, Tenable ASM, Palo Alto Cortex Xpanse, Microsoft Defender EASM, Hadrian, IONIX, Randori (IBM), Shodan Enterprise, and Bugcrowd ASM (the category leaders).

**Open-source emphasis**: ASM has a powerful open toolkit. **OWASP Amass**, the **ProjectDiscovery** suite (subfinder, httpx, nuclei, naabu), **reNgine**, and related recon frameworks enable fully self-hosted discovery and scanning. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Palo Alto Cortex Xpanse, Microsoft Defender EASM, Tenable ASM, Rapid7 Exposure Command](https://www.paloaltonetworks.com/cortex/cortex-xpanse)**  
  Enterprise external attack surface management from major security vendors—continuous discovery and exposure prioritization.

- **[Wiz, UpGuard, Detectify, Hadrian, IONIX](https://www.wiz.io/)**  
  Cloud and external exposure platforms combining asset inventory, misconfiguration detection, and continuous monitoring.

- **[Censys, Shodan Enterprise, Recorded Future ASI](https://censys.com/)**  
  Internet-wide scanning and intelligence platforms used for asset discovery and threat context.

- **[Assetnote, ProjectDiscovery Cloud, Bugcrowd ASM, NetSPI, Bishop Fox Cosmos, Randori](https://www.assetnote.io/)**  
  Specialist ASM and offensive-security oriented platforms for high-fidelity discovery and testing programs.

- **[Other commercial ASM platforms](https://www.paloaltonetworks.com/cortex/cortex-xpanse)**  
  Additional continuous external monitoring and brand-protection offerings.

## Open-Source GitHub Projects

- **[OWASP Amass](https://github.com/owasp-amass/amass)**  
  Flagship open-source framework for attack surface mapping and external asset discovery—OSINT, DNS enumeration, and asset graph storage.

- **[ProjectDiscovery suite](https://github.com/projectdiscovery)**  
  De facto open-source recon toolkit: **subfinder** (subdomains), **httpx** (HTTP probing), **naabu** (ports), **nuclei** (templated vulnerability checks), **dnsx**, and more—scriptable and CI-friendly.

- **[reNgine](https://github.com/yogeshojha/rengine)**  
  Open-source automated reconnaissance framework with a web UI—orchestrates subdomain discovery, scanning, and findings for self-hosted ASM-style workflows.

- **[Faraday](https://github.com/infobyte/faraday)**  
  Open collaboration platform that aggregates findings from multiple recon/scan tools into a shared workspace.

- **[Nmap, Masscan & classic scanners](https://github.com/nmap/nmap)**  
  Foundational open port and service scanners used in nearly every ASM pipeline.

- **[Certificate Transparency tools (crt.sh clients, certspotter)](https://github.com/search?q=certificate+transparency+OR+crt.sh+client)**  
  Open clients for CT logs—often the richest passive source for subdomain discovery.

- **[BBOT, theHarvester & OSINT frameworks](https://github.com/blacklanternsecurity/bbot)**  
  Broader open recon frameworks that expand asset graphs beyond pure DNS.

- **[Nuclei templates ecosystem](https://github.com/projectdiscovery/nuclei-templates)**  
  Community vulnerability and misconfiguration templates that turn discovery into actionable exposure findings.

### Additional Strong Open-Source Options

- **Discovery**: Amass + subfinder for maximum coverage.
- **Probing**: httpx + naabu + Nmap.
- **Vulnerability context**: nuclei with curated templates.
- **Orchestration**: reNgine or custom pipelines on ProjectDiscovery tools.
- **Composable stacks**: CT + passive DNS → resolve → probe → nuclei → ticket/SOAR.
- Commercial ASM still leads in continuous global scanning, attribution, and enterprise reporting.

**Frameworks for building custom systems**:  
**Amass** + **ProjectDiscovery** (subfinder, httpx, nuclei) form the core open ASM toolkit; **reNgine** adds a UI.  
Commercial platforms (Xpanse, Defender EASM, Wiz, Censys, Detectify, etc.) provide continuous coverage and analyst workflows.  
Security teams often run open recon in-house and use commercial EASM for always-on monitoring. Fully open stacks are highly capable for authorized discovery and periodic assessments.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Only scan and enumerate assets you own or have explicit authorization to test. Unauthorized scanning can violate law and terms of service. Nuclei and active probes must be scoped carefully.
- Open-source tools offer transparency and control but require you to operate infrastructure and interpret results. Commercial ASM platforms shift continuous scanning and support to the vendor. Neither replaces a vulnerability management process and remediation ownership.

---

**Made for security engineers, ASM analysts, and teams reducing unknown internet exposure.**  
Let's expand open attack surface discovery while recognizing the continuous global coverage that leading commercial EASM platforms deliver.
