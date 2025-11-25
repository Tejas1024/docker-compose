# 2_yaml_basics.md

# 🧾 YAML Basics

YAML = "Yet Another Markup Language"
- Used for readable configuration (Docker, Kubernetes)

## Syntax Principles

- Key-value pairs with indentation (space, not tab)
country: India
course: DevOps
year: 2025

text

- Lists written with `-`
fruits:

papaya

mango

avocado

grapes

apple

text

- Nesting shown by indentation

---

## 🌐 Difference Between HTML, XML, YAML

| Feature     | HTML (HyperText Markup Language) | XML (eXtensible Markup Language) | YAML (Yet Another Markup Language) |
|-------------|----------------------------------|-----------------------------------|------------------------------------|
| Purpose     | Web page structure/design        | Structured data storage/transport | Config files for tools/services    |
| Tags        | Uses tags (<h1>, <p>)            | Custom tags (<plugin>)            | No tags, just key-value pairs      |
| Readability | Browser-focused, not human       | Verbose, somewhat readable        | Highly human-friendly, simple      |
| Usage       | Frontend web development         | API/data storage, configs         | Config (Docker, Ansible, K8s)      |

---

## 📝 Summary

- HTML → Web pages, XML → Data storage, YAML → Config
- YAML is highly readable for humans and preferred for modern workflows.
text
# 3_devops_tools.md

# ⚙️ List of Popular DevOps Tools

---

| Category            | Tools                                      | Purpose                          |
|---------------------|--------------------------------------------|-----------------------------------|
| Version Control     | Git, GitHub, GitLab                        | Track/manage code changes         |
| CI/CD               | Jenkins, GitHub Actions, CircleCI          | Automate build/test/deployment    |
| Containerization    | Docker, Docker Compose                     | Package/run apps in containers    |
| Orchestration       | Kubernetes                                 | Manage containers at scale        |
| Configuration Mgmt  | Ansible, Puppet, Chef                      | Automate server setup/config      |
| Monitoring          | Prometheus, Grafana                        | Track performance, uptime         |
| Cloud Platforms     | AWS, Azure, GCP                            | Deploy/scale in the cloud         |

---

# 🚀 DevOps Tool Categories

## 1. Basic Tools
- **Linux:** OS platform for most DevOps operations
- **Shell Scripting:** Automate tasks (deployments, monitoring)
- **Git:** Version control, collaboration (GitHub, GitLab)

## 2. Advanced Tools
- **Maven:** Builds Java projects, handles dependencies
- **Jenkins:** CI/CD pipeline creation, automation
- **Docker:** Container packaging/deployment
- **Kubernetes:** Orchestrates and scales containers

## 3. Cloud Providers
- **AWS (Amazon Web Services):** Largest provider, CI/CD, hosting, storage
- **GCP (Google Cloud Platform):** Big Data, AI, GKE (Kubernetes)
- **Azure (Microsoft Azure):** Enterprise cloud, DevOps integration