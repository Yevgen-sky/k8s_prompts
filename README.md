# k8s_prompts

  **/prompts**

У цій директорії розміщено портфоліо промптів, створених за принципами Prompt Engineering.
Кожен .txt файл містить детальний інструктивний промпт англійською мовою, який:

визначає роль (наприклад, Senior DevOps Engineer)

задає контекст

встановлює технічні обмеження

описує вимоги до вихідного YAML

визначає формат відповіді

містить покрокові інструкції

Ці промпти використовуються для генерації Kubernetes-маніфестів у папці /yaml.

  **/yaml**

Директорія містить готові Kubernetes YAML-маніфести, згенеровані або перевірені на основі промптів із папки /prompts.
Тут знаходяться приклади:

Pod манифести

Deployment-подібні конфігурації

Liveness/Readiness Probe

CronJob

Job

Multi-container Pod

VolumeMounts

Secrets та ConfigMaps

Resource limits/requests

Ці файли слугують практичними прикладами використання промптів та демонструють вміння працювати з Kubernetes.


___________________________________________________________________________________________________________________



  **/prompts**

This directory contains a complete Prompt Engineering portfolio, following best practices from Google’s Prompt Engineering guidelines.
Each .txt file includes a structured prompt that:

defines a role (e.g., Senior DevOps Engineer)

provides context

specifies technical constraints

outlines required YAML manifest characteristics

defines the output format

includes step-by-step instructions

These prompts are designed for generating Kubernetes manifests stored in the /yaml directory.

  **/yaml**

This folder includes ready-to-use Kubernetes YAML manifests created using the prompts from /prompts.
It contains examples of:

Pod manifests

Liveness/Readiness probes

VolumeMounts and volumes

CronJob

Job

Multi-container Pods

Secrets and ConfigMaps

Resource requests and limits

These files act as practical examples demonstrating Kubernetes expertise and AI-assisted infrastructure generation.
