
# SAP ChaRM - Overview

- Plugin sync SAP Normal Changes in SAP’s Change Request Management with Jira issues
- Fetch all Jira issues using the provided JQL Query , for each Jira issue plugin checks whether Charm ID is already there or not . If not , it creates a Charm ID for each issue 
- In user input , user specifies Custom field name in Jira where they have stored Transport ID 
- If Transport ID is not there , then in SAP status changes to “In Development” using the Charm ID
- Jira status and HCL Accelerate’s VSM status changes as the SAP Charm ID’s status changes 
- Charm ID and Transport ID will be shown as “labels” in HCL Accelerate
- Plugin will sync in every 5 min


## Compatibility

This plug-in requires UrbanCode Velocity version 2.5.0 and later.

## Versions

UrbanCode Velocity plug-in images are located in DockerHub. To view available versions, see the [UrbanCode
DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-bitbucket-cloud/tags).

## History

### Version 2.2.1

- Initial release: syncs SAP Normal changes with Jira issues


|Back to ...||Latest Version|SAP ChaRM |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[2.2.1](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-sap-charm/ucv-ext-sap-charm:1.0.1.tar.7z.001)|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
