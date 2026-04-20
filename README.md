# Argo CD (argo-cd)
Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes that automates the deployment of applications by using Git repositories as the source of truth for defining the desired application state. It supports multiple config management tools (Helm, Kustomize, Jsonnet, plain YAML), multi-cluster deployments, RBAC, SSO integrations, and a fully-loaded web UI. Part of the CNCF ecosystem and the Argo Project, governed by the Linux Foundation.

**URL:** [https://argoproj.github.io/cd/](https://argoproj.github.io/cd/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Continuous Delivery, Containers, Deployment, GitOps, Kubernetes, CNCF, Open Source

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-04-19

## APIs

### Argo CD API
The Argo CD REST API provides programmatic access to all Argo CD functionality including application management, cluster registration, repository configuration, project RBAC, account management, notifications, and settings. Authentication uses JWT bearer tokens obtained via the session endpoint.

**Human URL:** [https://argo-cd.readthedocs.io/en/stable/developer-guide/api-docs/](https://argo-cd.readthedocs.io/en/stable/developer-guide/api-docs/)

#### Tags:

 - Continuous Delivery, GitOps, Kubernetes, REST API

#### Properties

- [Documentation](https://argo-cd.readthedocs.io/en/stable/developer-guide/api-docs/)
- [OpenAPI](openapi/argo-cd-openapi.json)
- [GettingStarted](https://argo-cd.readthedocs.io/en/stable/getting_started/)
- [Authentication](https://argo-cd.readthedocs.io/en/stable/developer-guide/api-docs/#authentication)
- [APIReference](https://cd.apps.argoproj.io/swagger-ui)

## Common Properties

- [Website](https://argoproj.github.io/cd/)
- [Documentation](https://argo-cd.readthedocs.io/en/stable/)
- [GettingStarted](https://argo-cd.readthedocs.io/en/stable/getting_started/)
- [GitHubOrganization](https://github.com/argoproj)
- [GitHubRepository](https://github.com/argoproj/argo-cd)
- [Blog](https://blog.argoproj.io/)
- [ReleaseNotes](https://github.com/argoproj/argo-cd/releases)
- [ChangeLog](https://github.com/argoproj/argo-cd/blob/master/CHANGELOG.md)
- [CLI](https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd/)
- [SDK](https://github.com/argoproj/argo-cd/tree/master/pkg/apiclient)
- [Support](https://github.com/argoproj/argo-cd/issues)

## Features

| Name | Description |
|------|-------------|
| Declarative GitOps Delivery | Defines application deployment state in Git repositories and automatically reconciles cluster state to match. |
| Multi-Cluster Deployment | Deploy and manage applications across multiple Kubernetes clusters from a single control plane. |
| ApplicationSet Controller | Automates creation of Argo CD Applications from templates across many clusters and namespaces. |
| Multiple Config Management Tools | Supports Helm, Kustomize, Jsonnet, plain YAML, and custom plugins for application templating. |
| Web UI | Fully-loaded graphical interface for visualizing application sync status, resource trees, and deployment history. |
| RBAC and Multi-Tenancy | Fine-grained role-based access control with project-level isolation for multi-team environments. |
| SSO Integration | Built-in SSO support for OIDC, OAuth2, LDAP, SAML 2.0, GitHub, GitLab, Microsoft, and LinkedIn. |
| Automated Sync | Continuously monitors Git and automatically syncs application state to match the desired state. |
| Sync Hooks | PreSync, Sync, and PostSync hooks for complex rollout strategies including blue/green and canary. |
| Webhook Support | Receives webhooks from GitHub, GitLab, and Bitbucket for instant sync on push events. |
| Audit Trail | Complete audit log of all deployment events and configuration changes. |
| Health Assessment | Built-in and custom health checks for Kubernetes resources to assess application health status. |
| Notifications | Configurable notifications via email, Slack, and other channels on sync events and health changes. |
| GPG Commit Verification | Verifies GPG signatures on Git commits for enhanced supply chain security. |

## Use Cases

| Name | Description |
|------|-------------|
| Continuous Deployment to Kubernetes | Automate application releases to Kubernetes clusters with every Git commit triggering a reconciliation cycle. |
| Multi-Environment Promotion | Promote application versions across dev, staging, and production environments using Git branch strategies. |
| Multi-Cluster GitOps | Manage application deployments consistently across dozens of Kubernetes clusters from a central Argo CD instance. |
| Cluster Add-On Management | Automatically deploy infrastructure add-ons (CNI, CSI, monitoring) to all clusters using ApplicationSet. |
| Tenant Self-Service | Allow development teams to manage their own applications within project-scoped RBAC boundaries. |
| Disaster Recovery | Quickly restore application state to any prior Git commit in case of production incidents. |
| Compliance and Auditability | Maintain a complete audit trail of all deployment changes via Git history and Argo CD event logs. |

## Integrations

| Name | Description |
|------|-------------|
| Helm | Native support for Helm chart rendering and deployment with value overrides. |
| Kustomize | Native support for Kustomize overlays for environment-specific configuration. |
| HashiCorp Vault | Integrates with Vault for secret management using the argocd-vault-plugin. |
| GitHub Actions | Trigger Argo CD syncs or check sync status as part of GitHub Actions CI pipelines. |
| Jenkins | Integrate Argo CD sync steps into Jenkins CI/CD pipelines. |
| Prometheus | Exposes metrics for Prometheus scraping to monitor application sync health and performance. |
| Grafana | Pre-built dashboards for visualizing Argo CD metrics in Grafana. |
| Open Policy Agent | Enforce admission policies via OPA and Gatekeeper before Argo CD syncs resources. |
| Argo Rollouts | Native integration with Argo Rollouts for progressive delivery (canary, blue/green). |
| Argo Workflows | Trigger Argo Workflows as part of sync hooks for complex multi-step pipelines. |
| Slack | Send deployment notifications and alerts to Slack channels. |
| AWS EKS | Manage applications on Amazon EKS clusters with AWS IAM authentication support. |
| Google GKE | Deploy to Google Kubernetes Engine clusters with GKE authentication. |
| Azure AKS | Manage applications on Azure Kubernetes Service with Azure AD authentication. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Argo CD OpenAPI](openapi/argo-cd-openapi.json)

### JSON Schema

262 schema files in [json-schema/](json-schema/)

### JSON Structure

262 structure files in [json-structure/](json-structure/)

### JSON-LD

- [Account Context](json-ld/argo-cd-account-context.jsonld)
- [Application Context](json-ld/argo-cd-application-context.jsonld)
- [ApplicationSet Context](json-ld/argo-cd-applicationset-context.jsonld)
- [Cluster Context](json-ld/argo-cd-cluster-context.jsonld)
- [Project Context](json-ld/argo-cd-project-context.jsonld)
- [Repository Context](json-ld/argo-cd-repository-context.jsonld)
- [Session Context](json-ld/argo-cd-session-context.jsonld)
- [Notification Context](json-ld/argo-cd-notification-context.jsonld)
- [GPG Key Context](json-ld/argo-cd-gpgkey-context.jsonld)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Argo CD API](capabilities/shared/argo-cd-api.yaml) — 9 operations for GitOps application, cluster, repository, and project management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [GitOps Delivery](capabilities/gitops-delivery.yaml) | Argo CD | 9 | Platform Engineer, DevOps Engineer |

## Vocabulary

- [Argo CD Vocabulary](vocabulary/argo-cd-vocabulary.yaml) — Unified taxonomy mapping 10 resources, 9 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Argo CD Spectral Rules](rules/argo-cd-spectral-rules.yml) — 17 rules across 7 categories enforcing Argo CD API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
