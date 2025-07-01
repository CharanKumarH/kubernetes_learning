# Kubernetes Demo Project

This repository contains Kubernetes manifests for learning and deploying various types of Node.js and database-based applications.

---

## 📁 Directory Overview

- `db-demo-app/`  
  Contains deployment and service definitions for a database-backed demo app.

- `multi-container-seperate-pod/`  
  Multiple containers deployed in **separate pods** with related configurations.

- `multiple-container-deployment/`  
  Multiple containers deployed in the **same pod** using a single deployment.

- `test/`  
  Experimental YAMLs or submodule for testing.

---

## 📄 Key YAML Files

| File                          | Description                                  |
|------------------------------|----------------------------------------------|
| `all-in-one.yml`             | Single YAML for deployment + service         |
| `deployment-node-app.yml`    | Node.js app deployment                       |
| `nodeapp-config.yml`         | ConfigMap for Node.js app                    |
| `replica-set.yml`            | Example ReplicaSet configuration             |
| `service-node-app-demo.yml`  | Service for exposing Node.js app             |

---

## 📚 Learning Materials

- `Kubernetes.pdf` — PDF guide covering core K8s concepts.
- `kubemates notes.txt` — Plain text notes for quick reference.

---

## 🛠 Usage

```bash
# Apply all-in-one deployment
kubectl apply -f all-in-one.yml

# Or apply individual components
kubectl apply -f deployment-node-app.yml
kubectl apply -f service-node-app-demo.yml
