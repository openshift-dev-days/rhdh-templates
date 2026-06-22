# Parasol Insurance Development Environment

This template creates an isolated development environment for working on the Parasol Insurance application.

## What gets created

- A feature branch on your Parasol Insurance source repository
- A GitOps repository with deployment manifests and CI/CD pipeline configuration
- An ArgoCD Application to deploy and manage your development environment
- A catalog entry in Developer Hub to track your work

## CI/CD Pipeline

When you push code to your feature branch, the pipeline automatically:

1. **Clones** your source code
2. **Runs SonarQube SAST** for code quality analysis
3. **Builds and pushes** a container image to the registry
4. **Re-rolls out** the application with the updated image
