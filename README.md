# Kubernetes Prompt Engineering Portfolio  
This repository contains a collection of **Prompt Engineering examples for Kubernetes YAML manifest generation**.  
It was created as part of a DevOps assessment requiring:

- Mastery of **Prompt Engineering principles**
- Ability to generate clean, production-ready **Kubernetes manifests**
- Use of AI-assisted tools such as **kubectl-ai** from Google Cloud
- Demonstration of real-world DevOps automation patterns

All prompts are written in English and follow guidelines from **Google Prompt Engineering Whitepaper**:
- role specification  
- context  
- constraints  
- explicit output format  
- step-by-step reasoning instructions  

Each prompt generates one of the Kubernetes manifests located in `/yaml`.

---

## Repository Structure

```
k8s_prompts/
│
├── README.md
├── prompts/
│   └── *.txt   # Prompt Engineering scripts
└── yaml/
    └── *.yaml  # Kubernetes manifest outputs
```

---

# Prompt Documentation Table

| NAME | PROMPT | DESCRIPTION | EXAMPLE |
|------|--------|-------------|----------|
| **app** | [app.txt](prompts/app.txt) | Basic Pod manifest with container & port | [app.yaml](yaml/app.yaml) |
| **app-volumeMounts** | [app-volumeMounts.txt](prompts/app-volumeMounts.txt) | Pod with hostPath volume + probes | [app-volumeMounts.yaml](yaml/app-volumeMounts.yaml) |
| **app-configmap** | [app-configmap.txt](prompts/app-configmap.txt) | Pod consuming ConfigMap via env & volume | [app-configmap.yaml](yaml/app-configmap.yaml) |
| **app-cronjob** | [app-cronjob.txt](prompts/app-cronjob.txt) | CronJob running a scheduled command | [app-cronjob.yaml](yaml/app-cronjob.yaml) |
| **app-job** | [app-job.txt](prompts/app-job.txt) | Job with persistent disk + GCS rsync task | [app-job.yaml](yaml/app-job.yaml) |
| **app-livenessProbe** | [app-livenessProbe.txt](prompts/app-livenessProbe.txt) | Pod with liveness probe | [app-livenessProbe.yaml](yaml/app-livenessProbe.yaml) |
| **app-multicontainer** | [app-multicontainer.txt](prompts/app-multicontainer.txt) | Multi-container Pod sharing emptyDir | [app-multicontainer.yaml](yaml/app-multicontainer.yaml) |
| **app-readinessProbe** | [app-readinessProbe.txt](prompts/app-readinessProbe.txt) | Pod with readiness + liveness probes | [app-readinessProbe.yaml](yaml/app-readinessProbe.yaml) |
| **app-resources** | [app-resources.txt](prompts/app-resources.txt) | Pod with resource limits/requests | [app-resources.yaml](yaml/app-resources.yaml) |
| **app-secret-env** | [app-secret-env.txt](prompts/app-secret-env.txt) | Pod reading env vars from Secrets | [app-secret-env.yaml](yaml/app-secret-env.yaml) |
| **app-secret-volume** | [app-secret.txt](prompts/app-secret.txt) | Pod mounting Secret as volume | [app-secret.yaml](yaml/app-secret.yaml) |

---

# Prompt Engineering Approach

Each prompt applies the following structure:

1. **Role Specification**  
   Defines the model as a Senior DevOps/Kubernetes Engineer.

2. **Context**  
   Describes what the manifest must represent.

3. **Constraints**  
   Clear requirements, no comments, valid YAML only.

4. **Explicit Output Format**  
   YAML-only, correct indentation, kubectl-apply ready.

5. **Step-by-Step Instructions**  
   Ensures deterministic and reproducible output.

This demonstrates practical skills in:
- AI-assisted DevOps  
- Kubernetes automation  
- Infrastructure-as-code generation  
- Clean manifest design patterns  

---

# Using kubectl-ai (Google Cloud)

Prompts in this repository are compatible with Google Cloud’s **kubectl-ai** extension.

Install:

```bash
curl -fsSL https://raw.githubusercontent.com/GoogleCloudPlatform/kubectl-ai/main/install.sh | bash
```

Example usage:

```bash
kubectl ai generate deployment --image=nginx --replicas=2
```

This workflow aligns with the next-gen DevOps approach:  
**AI-assisted infrastructure generation and validation.**

---

# Contact / Submission

This repository is prepared for DevOps hiring assessment and includes all required deliverables:

- Prompt portfolio  
- Kubernetes YAML examples  
- AI-engineered manifest generation workflow  

For any additional details, feel free to reach out.

---

### ✔ Ready for review  
Thank you for taking the time to explore this prompt-engineering portfolio!

