# 🚀 Kubernetes Labs (In Progress)

## 📋 Overview
This repository contains hands-on Kubernetes configuration and deployment files for learning and practicing Kubernetes concepts. It includes cluster setup automation and multi-image deployments with various Kubernetes resources.

---

## 📁 Repository Structure

### 🔧 Cluster Setup
- **config.yml** - Kind cluster configuration file
  - 1 control-plane node (v1.35.1)
  - 2 worker nodes (v1.35.1)
  - Port mappings for HTTP (80) and HTTPS (443)

- **script.sh** - Automated Kind installation script

- **cron job.yml** - Cron job configuration

---

## 📦 Kubernetes Deployments

### 🌐 Nginx Folder
Nginx deployment configurations including:
- `daemonset.yml` - DaemonSet for node-level deployment
- `deployment.yml` - Deployment configuration
- `ingress.yml` - Ingress routing
- `namespace.yml` - Namespace isolation
- `physical-vol-claim.yml` - PersistentVolumeClaim
- `physical-vol.yml` - PersistentVolume
- `replicaset.yml` - ReplicaSet management
- `service.yml` - Service configuration
- `taintpod.yml` - Taints and Tolerations

### 🔌 Apache Folder
Apache deployment with advanced features:
- `deployment.yml` - Deployment configuration
- `hpa.yml` - Horizontal Pod Autoscaler
- `namespace.yml` - Namespace isolation
- `role.yml` - RBAC Role
- `role-binding.yml` - RBAC RoleBinding
- `service-account.yml` - Service Account
- `service.yml` - Service configuration

### 🗄️ MySQL Folder
MySQL stateful deployment:
- `configmap.yml` - ConfigMap for configuration
- `namespace.yml` - Namespace isolation
- `secrets.yml` - Secrets management
- `service.yml` - Service configuration
- `statefulset.yml` - StatefulSet for stateful workloads

---

## ✨ Key Features Implemented

✅ Multi-image Kubernetes deployments  
✅ Namespace isolation  
✅ RBAC (Role-Based Access Control)  
✅ Horizontal Pod Autoscaling (HPA)  
✅ PersistentVolumes and PersistentVolumeClaims  
✅ ConfigMaps and Secrets management  
✅ Ingress routing  
✅ DaemonSets and StatefulSets  
✅ Taints and Tolerations  
✅ Kind cluster automation  

---

## 🚀 Getting Started

1. **Create Kind cluster:**
   ```bash
   bash script.sh
   kind create cluster --config config.yml
   ```

2. **Deploy applications:**
   ```bash
   kubectl apply -f nginx/
   kubectl apply -f apache/
   kubectl apply -f mysql/
   ```

3. **Deploy cron jobs:**
   ```bash
   kubectl apply -f cron\ job.yml
   ```

---

## 📚 Learning Topics Covered

- Container Orchestration
- Kubernetes Manifests & YAML
- Deployments & ReplicaSets
- StatefulSets & DaemonSets
- Services & Ingress
- Storage: PV & PVC
- ConfigMaps & Secrets
- RBAC & Security
- Horizontal Pod Autoscaling
- Taints & Tolerations
- Namespace Management

---

## 📝 Notes

This is a learning/lab repository for hands-on Kubernetes practice. All configurations are implemented and tested.

---

**Status:** 🔄 In Progress
