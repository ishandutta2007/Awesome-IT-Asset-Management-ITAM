# Awesome-IT-Asset-Management-ITAM

## Top IT Asset Management (ITAM) Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Hardware Lifecycle Tracking, Software License Compliance & Self-Hosted ITAM Platforms*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **IT Asset Management (ITAM)**. These tools enable IT departments to track hardware and software assets throughout their lifecycle—knowing who has which laptop, when it was purchased, which licenses are available, and when renewals are due—while supporting compliance audits and financial planning.



**Examples** include ServiceNow Asset Management, Ivanti, Freshservice, ManageEngine AssetExplorer, Flexera One, Snow Software, Lansweeper, and Snipe-IT (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding per-asset SaaS pricing, and retaining full control over asset data—ideal for IT teams that need transparency, customization, and data sovereignty. The open-source landscape is anchored by **Snipe-IT** (the free, Laravel-based asset/license management standard), **GLPI** (the combined ITAM+ITSM platform with native inventory agent), and **Ralph** (the data-center-focused CMDB), with **OCS Inventory** serving as the discovery engine that feeds these systems.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ServiceNow Asset Management](https://www.servicenow.com/)**  

  The enterprise ITAM leader, ranked top overall in ISG's 2026 Buyers Guide with leadership in five categories . Deep CMDB integration, AI-driven discovery, and governance across hybrid environments. Enterprise-tier pricing. Best for large organizations already invested in ServiceNow's ITSM platform.



- **[Ivanti IT Asset Management](https://www.ivanti.com/)**  

  ISG-rated exemplary and a top-three overall leader in 2026 . Strong on automated asset discovery and configuration management aligned with ITSM workflows. Enterprise-priced. Best for organizations needing comprehensive ITAM with proven enterprise support.



- **[Freshservice (Freshworks)](https://www.freshworks.com/freshservice/)**  

  ISG-rated exemplary and top-three overall leader, with strong customer experience scores . Modern ITSM/ITAM platform with asset discovery, license management, and an approachable interface. Per-agent pricing. Best for mid-market teams wanting enterprise capability without enterprise complexity.



- **[ManageEngine AssetExplorer](https://www.manageengine.com/products/asset-explorer/)**  

  ISG-rated Innovative and a leader in Product Experience alongside ServiceNow and Ivanti . Comprehensive asset tracking, software license management, and reporting. Per-technician pricing with a free edition for small environments. Best for budget-conscious organizations needing solid ITAM fundamentals.



- **[Flexera One](https://www.flexera.com/)**  

  ISG-rated Exemplary, specializing in **Software Asset Management (SAM)** and cloud cost optimization . Strong for organizations facing software audits from vendors like Oracle and Microsoft. Enterprise-priced.



- **[Lansweeper](https://www.lansweeper.com/)**  

  ISG-rated Innovative . Powerful agentless network discovery scanning Active Directory, SNMP, SSH, and cloud environments. **Free tier** capped at 100 assets; paid Starter at $199/month for 2,000 assets . Best for MSPs and IT teams needing automated discovery before committing to full ITAM.



## Open-Source GitHub Projects



- **[Snipe-IT](https://github.com/snipe/snipe-it)**  

  **The free open-source IT asset/license management standard.** Built on Laravel (currently Laravel 11), web-based, and deployable on any Linux/Windows/macOS server with a Docker image available . **Core features**: hardware lifecycle tracking (who has which laptop, purchase dates for depreciation), software license management, accessories, consumables, and components. **REST API** enables third-party integrations including a **MCP Server** for AI agent access, PowerShell wrapper, Jira Service Desk plugin, and sync scripts for Jamf, Kandji, Mosyle, and UniFi . **Trade-offs**: no built-in discovery agent—data must be entered manually or via scripts; limited software license compliance workflows compared to enterprise tools . Best for IT teams wanting a straightforward, self-hosted asset tracker without per-asset fees.



- **[GLPI](https://github.com/glpi-project/glpi)**  

  **The combined ITAM + ITSM platform.** Merges asset management with a helpdesk, change management workflows, and—from version 10—a **native GLPI Agent** that discovers hardware and software inventory across Windows, Linux, and macOS endpoints without third-party tooling . **Plugin ecosystem** extends functionality with license management, reporting, and external integrations. **Trade-offs**: configuration overhead is real—requires agent setup, database tuning, and investment in defining asset categories before data becomes actionable. Underestimating the learning curve is a common reason deployments stall . Best for mid-size to large organizations needing asset tracking and service management in one platform, with engineering bandwidth to configure it properly.



- **[Ralph](https://github.com/allegro/ralph)**  

  **The data-center CMDB specialist.** Built by Allegro (Polish e-commerce company) for infrastructure teams managing physical data center assets—servers, network equipment, rack layouts, and the relationships between them . **CMDB-style modeling**: represent racks, mounted devices, network connections, and business services they support. **Well-structured REST API** enables infrastructure automation. **Trade-offs**: limited support for employee laptops, mobile devices, and office hardware; minimal software license management; no built-in discovery . Best for infrastructure and network operations teams with data-center-heavy environments needing relationship modeling and API-driven automation.



- **[OCS Inventory NG](https://github.com/OCSInventory-NG/OCSInventory-Server)**  

  **The discovery engine.** Agent-based and agentless network scanning that collects hardware specs, installed software, and network configuration from Windows, Linux, macOS, and Android endpoints . **Best paired with GLPI**: OCS handles scanning, GLPI handles management—a well-established open-source pattern . **Trade-offs**: dated web interface, basic reporting, and thinner community support than GLPI or Snipe-IT . Best for organizations needing automated inventory across large networks without manual entry.



### Additional Strong Open-Source Options



- **i-doit** — ITIL-aligned CMDB with relationship modeling and impact analysis. Best for ITSM teams needing documented dependency graphs for compliance and change management .

- **FusionInventory** — Agent-based discovery tool that integrates with GLPI. Best for teams wanting flexible inventory collection feeding multiple systems .

- **NetBox** — IPAM/DCIM platform for network infrastructure documentation. Not a SAM tool by design, but extensible via custom fields for software asset tracking .

- **Frameworks for building custom systems**: Use **Snipe-IT** for straightforward asset/license tracking with API integrations. Pair **OCS Inventory** with **GLPI** for automated discovery plus full ITAM/ITSM. Use **Ralph** for data-center CMDB needs with API automation. For ITIL CMDB requirements, add **i-doit**.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Open-source ITAM requires operational commitment**: self-hosted tools mean you own updates, database migrations, backups, and security patching. None provide built-in endpoint health telemetry comparable to commercial DEX platforms .

- **Discovery is not automatic in Snipe-IT or Ralph**: data must be populated via API, scripts, or manual entry. Pair with OCS Inventory or GLPI Agent for automated collection .

- **GLPI's configuration overhead is significant**: budget time for agent deployment, database tuning, and asset taxonomy definition before expecting actionable data .



---



**Made for IT administrators, MSPs, and organizations that want control over their asset inventory without per-asset fees.**  

Let's make IT asset management more open, transparent, and appropriately scoped.
