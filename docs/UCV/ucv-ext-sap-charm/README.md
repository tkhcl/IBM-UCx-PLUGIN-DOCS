
# SAP ChaRM

- Fetches the Jira issues , for each Jira issue plug-in checks whether ChaRM ID is already there or not . If not , it creates a ChaRM ID for each issue
- In user input , user specifies Custom field name in Jira where they have stored Transport ID
- If Transport ID is not there ,it can generate multiple Transport IDs in SAP as per requirement and then in Jira status changes to "In Development" using the ChaRM ID
- Jira status and UrbanCode Velocity's VSM status changes as the SAP ChaRM ID's status changes
- ChaRM ID and Transport ID will be shown as "Description" in UrbanCode Velocity
- plug-in will sync in every 5 min
- Please [contact](https://www.ibm.com/mysupport) the support team for plug-in installation

|Back to ...||Latest Version|SAP ChaRM ||
| :---: | :---: | :---: | :---: | :---: | 
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[2.2.1](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-sap-charm/ucv-ext-sap-charm:1.0.1.tar.7z.001)|[Overview](overview.md)|[Downloads](downloads.md)|
