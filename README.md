# 💠 Azure ARM Templates Collection

This repository contains a collection of Azure Resource Manager (ARM) templates and automation scripts I use across various cloud projects. These templates help automate and standardize Azure resource deployments ranging from networking to compute, storage, and governance.

> 🛠️ Some templates are production-ready, while others serve as quick-start references or experiments.

---

## 📁 Repository Structure

basic overview - feel free to explore

```plaintext
arm/
├── automations/                # Scripts, deployments, logic apps
├── template/                  # Full deployment scenarios (optional)
  └── templatespecs-examples/  # Full deployment scenarios (optional)

```
---

## 🚀 How to Use

You can deploy any ARM template using the Azure CLI:
```
az deployment group create \
  --resource-group <your-rg> \
  --template-file ./path/to/template.json \
  --parameters ./path/to/parameters.json
  ```