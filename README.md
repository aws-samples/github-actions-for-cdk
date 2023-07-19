## Github Action Workflow for CDK Deployment

This Github Actions workflow provides basic build, lint, test, deploy functionality to a Github Action workflow.

### What it does

1. Authenticates AWS account access to your deployment account using IAM role ARN defined in Github environmental variables
2. Performs authentication using OIDC auth
3. Builds all CDK, running all local build scripts
4. Performs static code linting and security checks
5. Deploys your CDK application in a single region
6. Deploys your CDK application in multiple regions
7. Deploys your CDK application using a user-defined e2e testing pipeline
8. Cleans up all resources

The above items must successfully pass for the workflow to execute successfully.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
