
Salesforce - Usage
==================

# Usage



### Usage




 


[Salesforce Integration with IBM UrbanCode 
Deploy](https://developer.ibm.com/urbancode/2017/05/02/salesforce-integration-ibm-urbancode-deploy/)

===============================================================================================================================================



[Example: Deploy Recent Validation ID](#example-deploy-recent-validation-id)

============================================================================




### Example: Deploy a Recent Validation
 ID




 



Version 5 of the plug-in introduces the ability to deploy a recent validation. Deploying a validation 
allows you to deploy faster by not rerunning tests associated with a deployment that was already validated. 
A 
validation does not complete the deployment process to the organization. A validation is used to check the success or 
failure messages that you would receive with an actual deployment. To validate your deployments, add the checkOnly=true 
parameter in your deploy step. 


[![](quick-deploy.png)](quick-deploy.png)
Example Deploy step with Check Only set to 
true




This will cause the step to set the recentValidationId as an output property. From here, we can reference it in
 a Deploy Recent Validation step using ``${p:[Deploy Step Name]/recentValidationId}``.



[![](deploy-recent-
validation.png)](deploy-recent-validation.png)
Example Deploy Recent Validation step references a recentValidationId







|Back to ...||Latest Version|Salesforce ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[9.1101988](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/SalesForce/salesforce-9.1101988.zip)|[Readme](README.md)|[Overview](overview.md)|[Steps](steps.md)|[Downloads](downloads.md)|
