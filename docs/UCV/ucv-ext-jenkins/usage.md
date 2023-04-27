
# Jenkins - Usage

The Jenkins plug-in provides features that can be used for the following purposes:

* Using Jenkins jobs as input for the release pipelines.
* Using Jenkins jobs as automation tasks in deployment plans.

The tables in the Configuration properties describe the properties to define the integration.

To install the plug-in, perform the following steps:

1.	From the home page, **click Settings > Integrations > Available**.
2.	In the **Action** column for the Jenkins plug-in, click **Install**.

To integrate the plug-in, perform the following steps:

1.	From the home page, click **Settings > Integrations > Installed**.
2.	In the **Action** column for the Jenkins plug-in, click **Add Integration**.
3.	On the Add Integration page, enter values for the fields used to configure the integration and define communication.
4.	Click **Save**.

## Using Jenkins jobs as input for the release pipelines

To use Jenkins jobs as input for the release pipelines, perform the following steps:
1. Log in to HCL Accelerate.
2. Click **Value streams** on the Navigation bar.
3. Click **All Value Streams** tab and select the required value stream.
4. On the Value Streams page, click **Pipeline** tab and then click **Add app** to add an application.
   The Add app - Choose the app dialog box opens.
5. In the **Managed by drop-down** list, select **Jenkins**.
6. In the **Application name** field, enter the application name.
7. In the **Description** field, enter the description for the application.
8. Click **Save** to add the application.
9. On the Jenkins application, in the **Input** column, click the **+** button to create a version.
   The Create version dialog opens.
10. Select the Jenkins job and then click **Save** to create a version.


## Using Jenkins jobs as automation tasks in deployment plans

To use Jenkins jobs as automation tasks in deployment plans, perform the following steps:

1. Log in to HCL Accelerate. 
2. Click **Releases** on the Navigation bar.
3. Click the required release.
4. On the Releases page, click the required deployment plan to open the deployment plan page.
5. On the deployment plan page, click **Create Task**.
   The Create task dialog box opens.
6. In the **Type** drop-down list, select **Jenkins**.
7. In the **Name** field, enter a task name.
8. In the **Description** field, enter the description of the task.
9. In the **Integration** drop-down list, select required integration for the task.
10. In the **Process** drop-down list, select required process for the task.
11. Select the **Wait** checkbox to wait for job to finish in Jenkins.
12. Perform any of the following step:
    * Click **Save** to save the task and close the dialog. 
    * Click **Save and create** another to save the task and create another task.


|Back to ...||Latest Version|Jenkins |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[1.0.4](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-jenkins/ucv-ext-jenkins:1.0.4.tar.7z.001)|[Readme](README.md)|[Overview](overview.md)|[Downloads](downloads.md)|
