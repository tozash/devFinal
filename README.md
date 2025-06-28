# DevOps Final Project

## 🏗️ Stack
| Service | Tech | Purpose |
|---------|------|---------|
| frontend | React + Nginx | UI |
| backend  | Node (Express) | API |
| prometheus | Prometheus v2.53 | Metrics |
| grafana | Grafana v11 | Dashboards |

## 🚀 Setup (Local)
```bash
git clone https://github.com/you/repo.git
cd compose
cp .env.example .env   # add secrets
docker compose up --build
```

## 📊 Monitoring

![Dashboard screenshot](docs/imgs/grafana-dashboard.png)

## 🔒 Security

Trivy scans located in `docs/imgs`. No critical CVEs after mitigation.

## 💥 Incident & Post-Mortem

See [`docs/postmortem.md`](docs/postmortem.md).

## 🤖 Automation

Optional Ansible playbook in `ansible/`.
