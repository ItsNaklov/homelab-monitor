# homelab-monitor 🖥️

Production-style monitoring stack for a private Kubernetes (K3s) homelab — fully automated using Terraform and CI/CD.

---

## ⚡ Highlights

- Kubernetes-based monitoring (Prometheus + Grafana)
- Infrastructure as Code with Terraform
- Automated deployment via GitHub Actions
- Secure access using Tailscale VPN
- Fully reproducible setup

---

## 📸 Dashboard Preview

![Dashboard Preview](./screenshots/dashboard.png)

---

## 🎯 Purpose

This project solves a common issue in homelab environments:

Monitoring setups are often manual, fragile, and not reproducible.

This implementation provides a fully automated and declarative monitoring stack, similar to real-world DevOps environments.

---

## 🏗️ Architecture

![Architecture](./screenshots/Architecture.png)

---

## 🛠️ Stack

**Infrastructure**

- K3s (Kubernetes)

**Observability**

- Prometheus
- Grafana
- node-exporter

**Automation**

- Terraform
- GitHub Actions

**Networking**

- Tailscale

---

## 🚀 Deployment

### Manual

```
cd terraform
terraform init
terraform apply
```

### CI/CD

```
git push origin main
```

---

## 📊 Observability

- node-exporter → system metrics (CPU, memory, disk)
- custom app → application-level metrics

---

## 🔐 Security

- Private network (no public exposure)
- Tailscale VPN access
- Secrets managed in CI/CD

---

## 📚 Concepts

- Infrastructure as Code
- GitOps workflow
- Idempotent deployments
- Observability stack
