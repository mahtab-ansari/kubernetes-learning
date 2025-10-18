# 🧩 Week 1 — Kubernetes Fundamentals (Pods, Deployments, Services)

| Day | Focus | Study Tasks | Hands-on Labs | Time |
|-----|--------|--------------|----------------|------|
| 1 | **Cluster Architecture** | [Understand K8s Components](https://kubernetes.io/docs/concepts/overview/components/) — API Server, etcd, Controller, Scheduler, Kubelet, Proxy | Install [Minikube](https://minikube.sigs.k8s.io/docs/start/) or [Kind](https://kind.sigs.k8s.io/docs/user/quick-start/); run `kubectl get nodes` | 2–3h |
| 2 | **Pods** | [Pods Concept](https://kubernetes.io/docs/concepts/workloads/pods/) & YAML basics | Create pods using `kubectl run` & YAML; view logs | 2–3h |
| 3 | **Deployments & ReplicaSets** | [Deployments](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) — rolling updates, rollbacks, scaling | Scale & update deployments | 2–3h |
| 4 | **Namespaces & Contexts** | [Namespaces](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/); kubeconfig | Create/switch namespaces; manage contexts | 2–3h |
| 5 | **Services** | [Service Types](https://kubernetes.io/docs/concepts/services-networking/service/) — ClusterIP, NodePort, LoadBalancer | Expose a deployment; test with `curl` | 2–3h |
| 6 | **Troubleshooting** | Learn `kubectl logs`, `describe`, Events | Debug broken pods (imagePullBackOff, CrashLoopBackOff) | 5h |
| 7 | **Review + KodeKloud Labs** | [Kubernetes Basics Course](https://kodekloud.com/courses/kubernetes-for-the-absolute-beginners-hands-on/) | Complete beginner labs & mini-quiz | 5h |

✅ *Checkpoint: You should now understand the Pod → Deployment → Service workflow.*

---

# 🛠️ Week 2 — CKA Core: Scheduling, Maintenance, Storage

| Day | Focus | Study Tasks | Hands-on Labs | Time |
|-----|--------|--------------|----------------|------|
| 8 | **Scheduling** | [Pod Scheduling](https://kubernetes.io/docs/concepts/scheduling-eviction/assign-pod-node/) — labels, taints, tolerations | Schedule pods using node selectors | 2–3h |
| 9 | **Static Pods** | [Static Pod Management](https://kubernetes.io/docs/tasks/configure-pod-container/static-pod/) | Create static pod under `/etc/kubernetes/manifests` | 2–3h |
|10 | **DaemonSets & Jobs** | [DaemonSets](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/) & [Jobs](https://kubernetes.io/docs/concepts/workloads/controllers/job/) | Create DaemonSet, CronJob | 2–3h |
|11 | **ConfigMaps & Secrets** | [ConfigMaps](https://kubernetes.io/docs/concepts/configuration/configmap/) & [Secrets](https://kubernetes.io/docs/concepts/configuration/secret/) | Mount ConfigMap & Secret as env vars | 2–3h |
|12 | **Resource Limits & Quotas** | [Resource Management](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/) | Create LimitRange & ResourceQuota | 2–3h |
|13 | **etcd Backup & Restore** | [Backup etcd](https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/) | Run `etcdctl snapshot save` & `restore` | 5h |
|14 | **Cluster Upgrade + Mock** | Review [Cluster Admin Tasks](https://kubernetes.io/docs/tasks/administer-cluster/) | Partial CKA mock on [KodeKloud Labs](https://kodekloud.com/courses/certified-kubernetes-administrator-cka/) | 5h |

✅ *Checkpoint: Able to handle node scheduling, backups, and basic cluster admin tasks.*

---

# 💻 Week 3 — CKAD Focus: Application Design & Deployment

| Day | Focus | Study Tasks | Hands-on Labs | Time |
|-----|--------|--------------|----------------|------|
|15 | **Multi-Container Pods** | [Init & Sidecar Containers](https://kubernetes.io/docs/concepts/workloads/pods/init-containers/) | Create pod with sidecar for logs | 2–3h |
|16 | **Probes (Health Checks)** | [Probes](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/) | Add liveness & readiness probes | 2–3h |
|17 | **Volumes & PVCs** | [Volumes](https://kubernetes.io/docs/concepts/storage/volumes/) & [PVCs](https://kubernetes.io/docs/concepts/storage/persistent-volumes/) | Mount PVC into pods | 2–3h |
|18 | **Ingress & Services** | [Ingress Concepts](https://kubernetes.io/docs/concepts/services-networking/ingress/) | Deploy Nginx Ingress Controller & expose app | 3h |
|19 | **Config in Pods** | Review ConfigMap & Secret usage | Inject configs via env vars & mounted volumes | 2–3h |
|20 | **Security & RBAC** | [RBAC Authorization](https://kubernetes.io/docs/reference/access-authn-authz/rbac/) | Create Role, RoleBinding, ServiceAccount | 5h |
|21 | **CKAD Mock Exam** | Simulate CKAD test (e.g., [Killer.sh](https://killer.sh)) | Full practice exam; review mistakes | 5h |

✅ *Checkpoint: Should be confident creating YAML from scratch & debugging apps.*

---

# ⚙️ Week 4 — Advanced Topics, Speed & Mock Exams

| Day | Focus | Study Tasks | Hands-on Labs | Time |
|-----|--------|--------------|----------------|------|
|22 | **Network Policies** | [Network Policies](https://kubernetes.io/docs/concepts/services-networking/network-policies/) | Apply ingress & egress restrictions | 2–3h |
|23 | **RBAC Deep Dive** | ClusterRoles, RoleBindings | Assign restricted access for users | 2–3h |
|24 | **Monitoring & Logging** | [Metrics Server](https://kubernetes.io/docs/tasks/debug/debug-cluster/resource-metrics-pipeline/) | Install metrics-server & use `kubectl top` | 2–3h |
|25 | **Imperative Commands** | [Kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/) | Practice fast YAML generation with `kubectl run` | 2–3h |
|26 | **Mock Exam: CKA** | Full CKA simulation (Killer.sh / KodeKloud) | Review cluster tasks & troubleshooting | 5–6h |
|27 | **Mock Exam: CKAD** | Full CKAD simulation | Reattempt failed questions | 5–6h |
|28 | **Review Weak Areas** | Focused revision (top 3 weak domains) | Hands-on labs retry | 2–3h |
|29 | **Rapid Revision** | Time yourself for 1-hour test | Practice key YAMLs | 2–3h |
|30 | **Final Prep** | System setup, aliases, test docs navigation | Light review & rest | 1–2h |

✅ *Final Checkpoint:*  
- Scoring **≥80%** in mock tests  
- Confident in `kubectl` commands  
- Familiar with Docs navigation  

---

# ⚡ Bonus Section

### 🧰 Useful Resources
- 📘 **Docs:** [https://kubernetes.io/docs](https://kubernetes.io/docs)  
- 🧑‍💻 **Cheat Sheet:** [kubectl reference](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)  
- 🎓 **KodeKloud CKA Course:** [Certified Kubernetes Administrator (CKA)](https://kodekloud.com/courses/certified-kubernetes-administrator-cka/)  
- 🎓 **KodeKloud CKAD Course:** [Certified Kubernetes Application Developer (CKAD)](https://kodekloud.com/courses/certified-kubernetes-application-developer-ckad/)  
- 🧪 **Exam Simulator:** [Killer.sh](https://killer.sh) (comes with official exam purchase)

### 🧩 Aliases for Speed
```bash
alias k=kubectl
complete -F __start_kubectl k
