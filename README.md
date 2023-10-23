# WordPress
About Acornfile for running WordPress on Acorn using Amazon RDS as a Database.

## Deploy the WordPress App 

You can deploy the sample web app on the Acorn SaaS Platform to test the Application.

## WordPress Acornfile

Let us have a close look at the Acornfile and see what is defined:

- **Containers**: These containers will be deployed for running WordPress. We have two containers, one for WordPress and the other for Redis. We are setting the environment variables returned from the Amazon RDS for the WordPress container.
- **Services**: Acron services are external services your application can utilize. In this case, we use the [Amazon RDS service from the catalog](https://aws.amazon.com/rds/).


## Steps

1. Login into the Acorn SaaS Platform using the Github Sign-In option with your Github user.
2. You can select the "Create Acorn" option to create new Acorns and deploy your Application.
3. Choose the source for deploying your Acorns
  * Select "From Acorn Image" to deploy the sample Application and select its Image
  * Provide any random name such as `web-app` and keeping Project's default Region, type in the below Acorn image and choose Create 
    ```bash
    ghcr.io/rohitg00/wordpress-rds:v1.0
    ```
4. the sample App is now provisioned on the Acorn SaaS Platform and is available for **up to 2 hours**.
5. Once the Acorn runs, you can access it by clicking the Endpoint or the redirect link.

## Acorn Nextcloud App Details

The Acorn Dashboard integrates multiple features such as Events, Logs, Details, and access to the Shell of the Application. Details include the CPU, Memory, Network, Latency, Requests, and Errors for the Application.

Explore various available options by clicking the Menu option on your Acorn App.

For more details on using the Acorn Dashboard, check this link - 

## Edit the Acorn Application

You can edit your Acorn's Image and Advanced Options by selecting the Edit option 

## Remove Acorn Application

Select the Remove option from your Acorn's Menu to Remove the Acorn.

