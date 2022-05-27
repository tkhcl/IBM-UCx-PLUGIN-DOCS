
IBM UrbanCode Release - Overview
================================

# Overview



### Overview




 


Use the IBM UrbanCode Release plug-in to manage the integration of IBM UrbanCode Deploy with IBM 
UrbanCode Release. The plug-in includes steps to retrieve the active release for an environment, add comments to tasks, 
add statuses to snapshots and updating the IBM UrbanCode Release inventory for an application.


To add the IBM 
UrbanCode Release plug-in steps to processes, click **IBM UrbanCode Release** in the step palette of the process editor.



This plug-in includes these steps:


* [Add Comment to Task](#install_application " Add Comment to Task")
* [Add 
Snapshot Status](#add_snap_shot_status "Add Snapshot Status")
* [Check Gate Status](#check_gate_status "Check Gate 
Status")
* [Get Release for Environment](#get_release_for_environment "Get Release for Environment")
* [Sync 
Snapshot](#sync_snapshot "Sync Snapshot Status")
* [Update Application](#update_application "Update Application")


### 
Compatibility


This plug-in requires IBM UrbanCode Deploy version 6.0.1.2 or later.


This plug-in runs on all 
operating systems that the IBM UrbanCode Deploy agent supports except for IBM z/OS.


### Installation


No special 
steps are required for installation. See [Installing plug-ins in UrbanCode 
Deploy](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in UrbanCode 
Deploy").


### History


#### Version 9


Version 9 includes the following changes:


* The Password property is now a 
secure field.
* Added HTTP statusLine and body responses for failed Status Snapshot deployments in the Add Snapshot 
Status step.


#### Version 8


Version 8 includes the following change:


* Support property file encryption.


#### 
Version 7


Version 7 includes the following changes:


* Revised descriptions and names.
* A check for valid UUID in 
the Check Gate Status step


#### Version 5


Version 5 includes the Check Gate Status step, which checks lifecycle 
phase gates when deploying in IBM UrbanCode Deploy.


#### Version 4


Version 4 fixes a defect with compatibility with 
IBM UrbanCode Deploy 6.1.0.4 and later.




|Back to ...||Latest Version|IBM UrbanCode Release ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[9.1056530](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/ucr-plugin/ucr-plugin-9.1056530.zip)|[Readme](README.md)|[Usage](usage.md)|[Steps](steps.md)|[Downloads](downloads.md)|
