# Terraform Infrastructure as Code (IaC)# Terraform Infrastructure as Code (IaC)

Este repositório contém a definição de infraestrutura como código (IaC) utilizando **Terraform**, seguindo boas práticas de **segurança, modularização, versionamento e conformidade**, com validação automatizada via **Checkov**.

## 📌 Objetivo

Provisionar e gerenciar infraestrutura de forma **segura, previsível e auditável**, garantindo:
- Padronização
- Reprodutibilidade
- Segurança por padrão (security by default)
- Compliance automatizado

---

## 🏗️ Estrutura do Repositório

```text
.
├── modules/            # Módulos reutilizáveis
│   └── vpc/
│       ├── main.tf
│       ├── variables.tf
│       └── outputs.tf
├── environments/
│   ├── dev/
│   │   ├── main.tf
│   │   ├── backend.tf
│   │   └── terraform.tfvars
│   ├── staging/
│   └── production/
├── providers.tf
├── versions.tf
├── variables.tf
├── outputs.tf
├── .checkov.yml
├── .gitignore
└── README.md
