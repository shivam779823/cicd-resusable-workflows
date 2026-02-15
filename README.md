| Layer     | Protection                    |
| --------- | ----------------------------- |
| Gitleaks  | Secret leaks                  |
| CodeQL    | Code vulns                    |
| pip-audit | Dependency CVEs               |
| Trivy     | Container CVEs                |
| SBOM      | Supply chain visibility       |
| Cosign    | Image integrity               |
| SLSA      | Build provenance              |
| OPA       | K8s misconfig prevention      |
| Kyverno   | Cluster admission enforcement |
| Argo CD   | Git as source of truth        |


🔐 Security Boundaries (Important)
Layer	Has Cluster Access?	Has Build Access?
GitHub Actions	❌ No	✅ Yes
Argo CD	✅ Yes	❌ No
Developers	❌ Direct cluster access not required	✅ Code access