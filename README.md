# Prompt Library

A reusable prompt library for generating production-ready software projects with strong coding standards, architecture, testing, security, and deployment practices.

## Library Structure

```text
prompt-library/
├── frontend/
│   ├── react-nextjs/
│   │   └── react-nextjs-fullstack.prompt.txt
│   └── angular/
│       └── angular-frontend.prompt.txt
├── backend/
│   ├── java-spring/
│   │   └── java-spring-backend.prompt.txt
│   └── python-fastapi/
│       └── python-fastapi-backend.prompt.txt
├── devops/
│   └── devops-infra.prompt.txt
├── cloud/
│   └── aws-deployment.prompt.txt
│   └── azure-deployment.prompt.txt
│   └── gcp-deployment.prompt.txt
```

## How to use

1. Choose the folder that matches your stack.
2. Open the corresponding prompt file.
3. Replace `<project-name>` with your project name.
4. Paste the prompt into your AI tool.
5. Generate the boilerplate and review the output for correctness, security, and maintainability.

## Prompt Index

### Frontend
- `frontend/react-nextjs/react-nextjs-fullstack.prompt.txt`
- `frontend/angular/angular-frontend.prompt.txt`

### Backend
- `backend/java-spring/java-spring-backend.prompt.txt`
- `backend/python-fastapi/python-fastapi-backend.prompt.txt`

### DevOps
- `devops/ci-cd/devops-infra.prompt.txt`

### Cloud
- `cloud/aws-deployment.prompt.txt`
- `cloud/azure-deployment.prompt.txt`
- `cloud/gcp-deployment.prompt.txt`

## Full Stack Composite Prompt (fullstack-composite.prompt.txt)

```text
You are generating a full-stack boilerplate project.

Create a production-ready full-stack project named <project-name> by combining:
- Frontend stack prompt
- Backend stack prompt
- DevOps/infrastructure prompt

Requirements:
- Generate a unified folder structure.
- Separate frontend, backend, and infra concerns cleanly.
- Ensure shared standards for linting, formatting, naming, testing, security, and deployment.
- Avoid duplication across the stack.
- Keep configuration centralized where appropriate.
- Include environment variable strategy across services.
- Include CI/CD and deployment guidance for the whole system.
- Produce a README describing the architecture, development workflow, and deployment flow.

Output:
1. Root folder structure.
2. Per-service folder structures.
3. Shared configuration files.
4. Service-specific starter files.
5. CI/CD and deployment files.
6. README.

Prefer a modular monorepo-style layout unless a different layout is explicitly requested.
```

## Incorporating these prompts into your project

```text
.github/
└── prompts/
    ├── standards.prompt.txt
    ├── quality-checklist.prompt.txt
    ├── folder-trees.prompt.txt
    └── fullstack-composite.prompt.txt
    └── ... the backend, frontend and devops prompts you need for your project
```
