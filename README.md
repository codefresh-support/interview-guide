# Codefresh Interview

The interview will be a live troubleshooting project based on the Codefresh project.  You can sign up beforehand (it is free), but we will send an invitation to our account for the interview. Below are some general items to review before the interview.

- Codefresh YAML
- Codefresh steps/plugins
- Git Triggers
- Variables
- Linux CLI
- Kubernetes / kubectl
- Helm / Helm CLI

## Interview Phases

Below is a description of what we will cover in each phase of the interview. Will provide aditional information during the interview as well.

### Phase 1 - YAML Validation

- Correct the provided YAML
- Make sure there are no Validation Errors

### Phase 2 - Misconfigurations

- Troubleshoot misconfigured steps (codefresh official steps)
- Use Variables instead of hardcoded items
- Organize the build into stages
- Add a Git trigger
- Add annotations

### Phase 3 - Kubernetes

- Create a namespace that is dynamic based on branch and commit id
- Deploy the file Kubernetes manifest 

### Phase 4 - Fault Tolerance

- Add items to steps to make sure the build won't fail
- Retry items as well

### Phase 5 - Helm (bonus)

- Create a namespace that is dynamic based on branch and commit id
- Deploy the helm chart with the built images from in the pipeline

## Names Of Contexts / Integrations

Docker: cf-support
Git: cf-support-bot
Kubernetes Cluster: k8s-interview

## Docker image

Images start with `cfsupport`. For example `cfsupport/mian:latest`

## Directory Structure of the Repository

.
├── LICENSE
├── README.md
├── codefresh.yml
├── db
│   ├── Dockerfile
│   └── words.sql
├── docker-compose.yml
├── kube-deployment.yml
├── web
│   ├── Dockerfile
│   ├── dispatcher.go
│   └── static
│       ├── angular.min.js
│       ├── app.js
│       ├── favicon.ico
│       ├── fonts
│       │   ├── font1.woff2
│       │   └── font2.woff2
│       ├── images
│       │   ├── dockercon-log.png
│       │   ├── homes.png
│       │   ├── lego_blue.png
│       │   ├── lego_light_blue.png
│       │   ├── lego_yellow.png
│       │   └── logo.svg
│       ├── index.html
│       └── style.css
├── words
│   ├── Dockerfile
│   ├── pom.xml
│   └── src
│       └── main
│           └── java
│               └── Main.java
└── wordsmith
    ├── Chart.yaml
    ├── templates
    │   └── kube-deployment.yml
    └── values.yaml
