This creates a CICD pipeline.

 - 1. Create an Azure App Service
 - 2. Download, open and copy the App service's Publish Profile.  
 - 3. Add a repo secret, with title "AZURE_WEBAPP_PUBLISH_PROFILE" and paste the Publish Profile.
 - 4. Update the CICD.yaml file in `.github/workflows` with the App name.

```yaml
env:
  AZURE_WEBAPP_NAME: your-app-name    # set this to your application's name
```
   
 Commit the changes and observe the buid, test and deploy. 
 View your site at <your_app_name>.azurewebsites.net
 