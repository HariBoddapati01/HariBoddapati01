<h1 align="center">Hari Boddapati</h1>

<p align="center">
  <b>Principal Platform / DevOps Engineer</b><br/>
  Kubernetes · Cloud-agnostic infrastructure · GitOps · Developer Experience
</p>

<p align="center">
  <a href="https://github.com/HariBoddapati01?tab=repositories"><img src="https://img.shields.io/badge/focus-Platform%20Engineering-2b6cb0?style=flat-square"/></a>
  <img src="https://img.shields.io/badge/Kubernetes-operators-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/IaC-GitOps-844FBA?style=flat-square&logo=terraform&logoColor=white"/>
</p>

---

### 👋 About

I build the **paved roads** that let application teams ship safely and fast — internal developer platforms, self-service infrastructure, and the guardrails that make "the right way" also "the easy way." My work sits where reliability, developer experience, and cloud economics meet.

I care about systems that are **boring on purpose**: idempotent, observable, and easy to reason about at 3 a.m.

- 🧭 **Platform engineering** — internal developer platforms, golden paths, self-service APIs
- ☸️ **Kubernetes** — operators & controllers, multi-tenancy, policy-as-code, workload isolation
- 🏗️ **Infrastructure as Code** — Terraform modules, GitOps (Argo CD / Flux), progressive delivery
- 🔭 **Reliability & observability** — SLOs, Prometheus/Grafana, actionable alerting
- 🔐 **Secure by default** — least-privilege RBAC, network policy, supply-chain hygiene

---

### 🚀 Featured project

#### [`kubtenant`](https://github.com/HariBoddapati01/kubtenant) — self-service multi-tenancy for Kubernetes

A Go operator (built on controller-runtime) that turns soft multi-tenancy into a single declarative `Tenant` CRD. It reconciles each tenant into fully guardrailed namespaces — **ResourceQuotas, LimitRanges, default-deny + allow-same-tenant NetworkPolicies, and owner RBAC** — all garbage-collected together via owner references.

```yaml
apiVersion: platform.hariboddapati.dev/v1alpha1
kind: Tenant
metadata: { name: acme }
spec:
  namespaces: [acme-dev, acme-staging, acme-prod]
  owners: [{ kind: Group, name: acme-platform-admins }]
  resourceQuota: { cpu: "16", memory: 32Gi, pods: "80" }
  networkIsolation: true
```

`idempotent reconciliation` · `native GC, no finalizers` · `distroless non-root image` · `race-tested, CI-gated`

---

### 🧰 Toolbelt

![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white)
![Helm](https://img.shields.io/badge/-Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Argo CD](https://img.shields.io/badge/-Argo%20CD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![GCP](https://img.shields.io/badge/-GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=HariBoddapati01&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&title_color=326CE5&icon_color=326CE5" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=HariBoddapati01&layout=compact&hide_border=true&langs_count=8&title_color=326CE5" alt="Top languages"/>
</p>

<p align="center"><i>Building reliable, self-service platforms — one paved road at a time.</i></p>
