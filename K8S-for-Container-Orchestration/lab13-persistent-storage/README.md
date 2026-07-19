# Lab 13 - Persistent Storage Setup for Application Logging

## Objective

Create a PersistentVolume (PV) and a PersistentVolumeClaim (PVC) to provide persistent storage for application logs.

---

## Prerequisites

- Docker
- Minikube
- kubectl

---

## Create Persistent Volume

Create the PersistentVolume.

```bash
kubectl apply -f persistent-volume.yaml
```

**Output**

![PV](screenshots/pv-create.png)

---

## Verify Persistent Volume

Verify that the PersistentVolume has been created successfully.

```bash
kubectl get pv
```

**Output**

![GET-PV](screenshots/get-pv.png)

---

## Create Persistent Volume Claim

Create the PersistentVolumeClaim.

```bash
kubectl apply -f persistent-volume-claim.yaml
```

**Output**

![PVC](screenshots/pvc-create.png)

---

## Verify Persistent Volume Claim

Verify that the PersistentVolumeClaim has been created successfully.

```bash
kubectl get pvc
```

**Output**

![GET-PVC](screenshots/get-pvc.png)

---

## Verify PV and PVC Binding

Verify that the PersistentVolume and PersistentVolumeClaim are successfully bound.

```bash
kubectl describe pv app-logs-pv

kubectl describe pvc app-logs-pvc
```

**Output**

![BOUND](screenshots/pv-pvc-bound.png)

---

## Result

- ✅ PersistentVolume created successfully.
- ✅ PersistentVolumeClaim created successfully.
- ✅ PV and PVC successfully bound.
- ✅ Persistent storage configured for application logging.