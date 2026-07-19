# Lab 12 - Managing Configuration and Sensitive Data with ConfigMaps and Secrets

## Objective

Store non-sensitive configuration using a ConfigMap and sensitive data using a Secret.

---

## Prerequisites

- Docker
- Minikube
- kubectl

---

## Create ConfigMap

Create the ConfigMap.

```bash
kubectl apply -f configmap.yaml
```

**Output**

![CONFIGMAP](screenshots/configmap-create.png)

---

## Verify ConfigMap

Verify that the ConfigMap has been created successfully.

```bash
kubectl describe configmap mysql-conf
```

**Output**

![CONFIGMAP-DESCRIBE](screenshots/configmap-describe.png)

---

## Create Secret

Create the Secret containing the database credentials.

```bash
kubectl apply -f secret.yaml
```

**Output**

![SECRET](screenshots/secret-create.png)

---

## Verify Secret

Verify that the Secret has been created successfully.

```bash
kubectl describe secret mysql-secret
```

**Output**

![SECRET-DESCRIBE](screenshots/secret-describe.png)

---

## Result

- ✅ ConfigMap created successfully.
- ✅ MySQL configuration stored in the ConfigMap.
- ✅ Secret created successfully using Base64-encoded values.
- ✅ Sensitive database credentials stored securely in the Secret.