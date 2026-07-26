# Azure Identity Governance: Agent Identity Blueprints vs. Access Packages

In Microsoft Entra ID (formerly Azure AD), **Agent Identity Blueprints** act as templates to automatically deploy managed identities with predefined permissions for AI agents, while **Access Packages** group resources into single bundles to manage human and service access lifecycle through requests and approvals.

---

### Core Differences

| Feature | Agent Identity Blueprints | Access Packages |
| :--- | :--- | :--- |
| **Primary Target** | AI workloads and autonomous agents | Employees, partners, and applications |
| **Main Purpose** | Standardization of AI security | Automated access requests and lifecycle |
| **Mechanism** | Code-driven templates (IaC) | Self-service portals and approval workflows |
| **Governance Focus** | Least-privilege blueprint compliance | Time-bound access and access reviews |

---

### Agent Identity Blueprints
* **AI automation**: Standardizes identity creation for autonomous AI agents and Copilot extensions.
* **Security Guardrails**: Hardcodes maximum permissible boundaries to prevent AI from escalating its own privileges.
* **Scalable deployment**: Integrates directly into Infrastructure as Code (IaC) pipelines for dev teams.

### Access Packages
* **Resource bundling**: Groups SharePoint sites, Azure roles, and groups into a single package.
* **Approval workflows**: Requires multi-stage manager or sponsor approvals before granting access.
* **Automatic expiration**: Revokes access automatically after a set duration to prevent privilege creep.
* **Access reviews**: Triggers recurring audits to ensure users still need their assigned access.
