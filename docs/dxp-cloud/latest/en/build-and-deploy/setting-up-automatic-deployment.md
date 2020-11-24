# Setting Up Automatic Deployment

You can speed up the deployment of CI builds by configuring the CI service to automatically deploy them to your Project's `dev` environment.

Follow these steps to set it up:

1. Navigate to the `infra` environment for your DXP Cloud Project.

1. Go to the *CI* service's page, and click on the *Environment Variables* tab.

   ![Go to the CI service's page, and click on the Environment Variables tab](./setting-up-automatic-deployment/images/01.png)

1. Add the following variable to the CI service:

   * **Key**: `DEVELOPMENT_BRANCH_NAME`

   * **Value**: enter the name of the branch you want to use for automatic deployments.

1. Click on *Save Changes*. This causes the CI service to restart with the new variable.

   ![After adding the DEVELOPMENT_BRANCH_NAME variable, click on Save Changes.](./setting-up-automatic-deployment/images/02.png)

Once restarted, any changes merged to your specified branch are automatically built and deployed to the `dev` environment.

## Additional Information

* [Overview of the DXP Cloud Development Workflow](./overview-of-the-dxp-cloud-deployment-workflow.md)
* [Deploying Changes via the DXP Cloud Console](./deploying-changes-via-the-dxp-cloud-console.md)
* [Deploying Changes via the CLI Tool](./deploying-changes-via-the-cli-tool.md)