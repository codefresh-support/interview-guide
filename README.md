# Codefresh Interview

The technical component of our interview is a troubleshooting project. This document outlines the steps involved. We do not require the full test to be completed, and it is your approach to solving problems and your learning process that we are most interested in.

As part of the interview process, we will send an invitation to a Codefresh account to you for you to join and some resources with additional instructions. 

Below are some general items to review before the interview.

- Codefresh YAML
- Codefresh steps/plugins
- Git Triggers
- Variables
- Linux CLI
- Kubernetes / kubectl
- Helm / Helm CLI

## Interview Phases

Below is a description of what we will cover in each phase of the interview. Will provide additional information during the interview as well.

### Phase 1 - Setup

- Accept the invitation to a Codefresh account
- Set up some external services
- Deploy Minikube
- Install the Classic Runner for Codefresh using a Helm chart

### Phase 2 - YAML Validation

- Correct the provided YAML
- Make sure there are no YAML Validation Errors

### Phase 3 - Misconfigurations

- Troubleshoot misconfigured steps (Codefresh official steps)
- Use Variables instead of hardcoded items
- Organize the build into stages
- Add a Git trigger
- Add annotations to built images

### Phase 4 - Kubernetes

- Dynamically create a namespace based on branch and commit id
- Deploy the app using Kubernetes manifest

### Phase 5 - Schedule the Next Interview

- Once you have reached this point, schedule the next interview stage with us, and feel free to continue.

### Phase 6 - Fault Tolerance

- Add items to steps to make sure the build won't fail on allowable errors
- Retry items as well

### Phase 7 - Helm (bonus points!)

- Dynamically create a namespace based on branch and commit id
- Deploy the helm chart with the built images from the pipeline

### Phase 8 - Documentation (bonus points!)

- Write up the technical steps you went through for Phase 1, part 7 as if you were explaining the process to a customer via email, blog post, or similar.


## Directory Structure of the Repository

```bash
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
```
