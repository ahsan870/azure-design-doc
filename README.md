# Azure Enterprise E-Commerce Architecture

An interactive design document for a secure, multi-tier e-commerce platform on Azure, with an interview-prep guide for Azure cloud migration projects.

**Live site:** https://ahsan870.github.io/azure-design-doc/

## What's inside

The site is a single page with four tabs:

| Tab | Contents |
|---|---|
| **Architecture Graph** | Interactive diagram: Front Door → App Gateway → APIM → three private AKS tiers → data stores, plus egress through Azure Firewall, Azure Monitor, and platform/ops tooling. Hover over a node to highlight its connections. |
| **Service Intro** | One card per Azure and third-party service and the role it plays. |
| **Readme** | The solution architecture and provisioning guide, in 19 sections: requirements, key decisions, IP plan, DNS, request flow and TLS, gateways, AKS, NSG and firewall rules, data, messaging, identity, security, observability, DR, CI/CD (GitHub or Azure DevOps), tool connectivity, cost, and risks. |
| **Interview Prep** | Migration roadmap, pre-migration checklist, an AWS / GCP / on-prem → Azure service map, and 40 Q&As (filter and search) covering migration and Azure architecture. |

## Viewing locally

Open `azure_enterprise_architecture.html` in a browser. There's no build step. Tailwind and Google Fonts load from their CDNs, so you need an internet connection.

## Notes

- Names such as `contoso.com`, East US 2 and Central US are placeholders.
- Items marked **TBD** in the doc need business sign-off before build.
- Vendor capabilities and dates (SKUs, retirements, Private Link availability) change. Check them against current documentation before you rely on them.
