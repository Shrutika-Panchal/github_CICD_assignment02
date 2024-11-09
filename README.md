# GitHub Actions CI/CD Pipeline Python App

## GitHub Actions Workflow

This repository uses GitHub Actions for Continuous Integration and Continuous Deployment (CI/CD). The workflow defined in the `.github/workflows` directory automatically runs when code is pushed to the `main` branch.

### Workflow Steps

The workflow performs the following steps:

1. **Build**: Installs dependencies, runs tests, and prepares the application for deployment.
2. **Deploy to Staging**: Deploys the application to a staging environment when changes are pushed to the `staging` branch.
3. **Deploy to Production**: Deploys the application to production when a release is tagged.

### Configuring Secrets

To configure the necessary secrets for deployment, follow these steps:

1. **EC2_HOST**: The hostname or IP address of your staging or production server.
2. **EC2_USERNAME**: The username for SSH access to your staging or production server.
3. **EC2_SSH_KEY**: The SSH private key used for authentication when deploying to your staging or production server.

Store these secrets in your GitHub repository settings:

1. Navigate to your repository on GitHub.
2. Go to the "Settings" tab.
3. Click on "Secrets" in the left sidebar.
4. Click on "New repository secret".
5. Enter the name and value for each secret.
6. Click on "Add secret" to save each secret.

Commit Changes: After adding or updating the instructions, commit the changes to the README.md file.

Push Changes: Push the committed changes to the main branch of your GitHub repository.

Once the changes are pushed, anyone accessing the repository will see the updated instructions in the README.md file, providing guidance on how the GitHub Actions workflow works and how to configure the necessary secrets.
