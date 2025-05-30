Choosing the right internal developer portal (IDP) is a critical decision for platform engineering teams. Most are looking to improve their developer experience, streamline software delivery, and adopt DevOps best practices. CNCF Backstage has become a popular open-source framework for building IDPs, but getting it right demands significant customization, manual plugin integration, and ongoing maintenance effort.

Red Hat Developer Hub, built on top of Backstage, offers a low maintenance enterprise-ready alternative. It's a carefully curated, fully supported, and production-hardened solution that's ideal for platform teams hoping to reduce the engineering burden associated with a CNCF Backstage. The matrix below highlights key differences between Red Hat Developer Hub and CNCF Backstage - so you can figure out which solution best aligns with your specific needs.

## Feature Comparison

| Feature | CNCF Backstage | Red Hat Developer Hub |
|--------|----------------|------------------------|
| Software Catalog | <span style="color:green">✔</span> | <span style="color:green">✔</span> |
| Software Templates (Scaffolder) | <span style="color:green">✔</span> | <span style="color:green">✔</span> |
| TechDocs | <span style="color:green">✔</span> | <span style="color:green">✔</span> |
| Global Search and Query | <span style="color:green">✔</span> | <span style="color:green">✔</span> |
| Kubernetes Helm-based Installer | <span style="color:green">✔</span> | <span style="color:green">✔</span> |
| Kubernetes Operator-based Installer | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Zero-Code solution (no need to maintain Backstage code) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| 24x7 Enterprise Support | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Supported on all major K8s platforms (GKE, AKS, EKS, OpenShift) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Enterprise Grade Security | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Secure RHEL-based UBI Container | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Fast-track Security Fixes (Rapid CVE resolution) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Authentication (e.g., Keycloak federated, Ping Federate) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Audit Logging (template/catalog actions) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Role-Based Access Control (RBAC) with GUI | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Workflow Automation Engine (Orchestrator) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Docker/Podman Local Installation (faster inner-loop development) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Dynamic Plug-Ins (no need to recompile) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Verified Plugin Compatibility | <span style="color:#e6c200">✘</span> (self-verify) | <span style="color:green">✔</span> |
| Extensions Catalog Plugin (marketplace) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| Adoption Insights Plugin (user metrics) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| 20+ Red Hat Plugins (e.g., Tekton, ArgoCD, Kiali, 3scale, ACS, Ansible) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
| [Free Software Templates Library](https://github.com/redhat-developer/red-hat-developer-hub-software-templates) | <span style="color:red">✘</span> | <span style="color:green">✔</span> |
