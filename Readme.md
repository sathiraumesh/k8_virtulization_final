# k8_virtulization_final

---

## ⚙️ Prerequisites

- A running Kubernetes cluster
- `kubectl` (v1.14+) and `kustomize` (built into `kubectl`)
- Docker image pushed to registry:  
  `your-registry/frontend:<tag>`
- Add your Docker Hub credentials encoded in **base64** in `kubernetes/.secrets/dockerconfigjson`
---

## 🟢 Deploy the Application

From the root or inside this folder:

```bash
cd kubernetes
kubectl apply -k .

Access the web application from `http://localhost:30000`

