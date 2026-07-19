# Kubernetes for Container Orchestration

This directory contains hands-on labs related to Kubernetes container orchestration completed during the iVolve Internship.

## Labs

### Lab 10

Node Isolation Using Taints in Kubernetes.

- Create a Kubernetes cluster with two nodes.
- Apply a taint to the worker node.
- Verify the taint using `kubectl describe`.

[Lab 10 - Node Isolation Using Taints](lab10-node-taints/)

---

### Lab 11

Namespace Management and Resource Quota Enforcement.

- Create a dedicated namespace.
- Apply a ResourceQuota to limit pod creation.
- Verify the quota configuration.
- Test quota enforcement by creating multiple pods.

[Lab 11 - Namespace and Resource Quota](lab11-resource-quota/)

---

### Lab 12

Managing Configuration and Sensitive Data with ConfigMaps and Secrets.

- Store non-sensitive configuration using a ConfigMap.
- Store sensitive database credentials using a Secret.
- Use Base64 encoding for secret values.
- Verify ConfigMap and Secret creation.

[Lab 12 - ConfigMaps and Secrets](lab12-configmaps-and-secrets/)