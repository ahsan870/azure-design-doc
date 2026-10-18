# Cloud Reference Architectures

Interactive design documents for one secure, multi-tier e-commerce platform, designed on each major cloud. Each version includes interview prep for cloud migration projects.

**Live site:** https://ahsan870.github.io/azure-design-doc/

| Cloud | Page | Status |
|---|---|---|
| Azure | [`azure/index.html`](azure/index.html) | Complete |
| AWS | [`aws/index.html`](aws/index.html) | Complete |
| Google Cloud | [`gcp/index.html`](gcp/index.html) | Coming soon |

## What's on each cloud page

A cloud switcher (Azure | AWS | GCP) sits in the header of every page. Each cloud page has four tabs:

| Tab | Contents |
|---|---|
| **Architecture Graph** | Interactive diagram: edge → private L7 gateway → API gateway → three private Kubernetes tiers → data stores, plus egress inspection, native observability and platform/ops tooling. Hover over a node to highlight its connections. |
| **Service Intro** | One card per service and the role it plays. |
| **Readme** | The solution architecture and provisioning guide, in 19 sections: requirements, key decisions, accounts/landing zone and IP plan, DNS, request flow and TLS, gateways, Kubernetes, network rules, egress, data, messaging, identity, security, observability, DR, CI/CD, tool connectivity, cost, and risks. |
| **Interview Prep** | Migration roadmap, pre-migration checklist, service mapping into that cloud, and 40 Q&As (filter and search) covering migrations from the other clouds and on-prem, plus architecture questions. |

## Repository layout

```
index.html                           Landing page (choose a cloud)
azure/index.html                     Azure design + interview prep
aws/index.html                       AWS design + interview prep
gcp/index.html                       Google Cloud placeholder
azure_enterprise_architecture.html   Redirect for the original URL
```

## Viewing locally

Open `index.html` in a browser. There's no build step. Tailwind and Google Fonts load from their CDNs, so you need an internet connection.

## Notes

- Names such as `contoso.com` and `example.com`, and the Regions used, are placeholders.
- Items marked **TBD** need business sign-off before build.
- Vendor capabilities and dates (SKUs, retirements, regional availability) change. Check them against current documentation before you rely on them.
