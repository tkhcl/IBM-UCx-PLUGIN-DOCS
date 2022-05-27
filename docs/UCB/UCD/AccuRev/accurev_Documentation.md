
AccuRev - Documentation
=======================

# Overview




### Overview




 


AccuRev provides version control of source code. It contains features that allow developers to 
work independently, share code, maintain separate code branches for parallel projects and at the same time use a base 
stream containing the latest updates.


The AccuRev plug-in integrates IBM UrbanCode Build with AccuRev and automates 
populating a AccuRev workspace as part of a build process.. The plug-in provides integration properties, that define the
 connection between the UrbanCode Build server and AccuRev repository. For details, see 
[Repositories](http://www.ibm.com/support/knowledgecenter/SS8NMD_6.1.2/com.ibm.ucbuild.doc/topics/settings_project_repo_cpt.html).
 


The repository is configured based on a workflow.


### Compatibility


The plug-in runs on any agents that the IBM 
UrbanCode Build server supports.


This plug-in run on all supported IBM UrbanCode Build platforms.


### Installation



No special steps are required for installation. See [Installing plug-ins in 
UrbanCode](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in 
UrbanCode") products.


### History


#### Version 6.752929 released on March 9, 2016


Version 6.752929 includes the 
following features and fixes:


* Added RPX dependency.
* Translation for step information.
* Added support for using 
the transaction ID in the Changelog step.


#### Version 5.669681


Version 5.669681 includes the following features and
 fixes:


* Updated to append the depot name to all change IDs. This prevents an issue where multiple depots can have 
the same change ID causing issues to get picked up for depots that do not contain them.


#### Version 4.604289



Version 4.604289 includes the following features and fixes:


* Fixed a communication issue where the UrbanCode Build 
server would fail if it was running with an IBM JDK or JRE.


# Settings




### Settings




 



The following settings are available when you import component versions by using the AccuRev 
plug-in. 




*Repository properties*  | Name | Type | Description |
| --- | --- | --- |
| Command Path | String | The 
location of the AccuRev command executable file, if the location is not specified on the system PATH statement. |
| 
Depot Name | String | The name or ID of the AccuRev depot. The depot is the repository on the server for all related 
source code. The value for this property can be used as part of the sourceconfig stream name with 
**``${source/repo/depotName}``**. If set, this will be recorded with any source changes for use by the AccuWork plug-in.
 |
| Password | Password | The password to be used to connect to the AccuRev server. |
| Password Script | String | The 
property to use for the password to connect to the AccuRev server. For example: ``${p:AccuRevPassword}``. If this 
property is specified, do not specify a value for thePassword property. |
| Repository Host | String | The location of 
the AccuRev server. Specify in the format: `host:port`. |
| User Name | String | The user name to be used to connect to 
the AccuRev server. |




*Integration properties*  | Name | Type | Description |
| --- | --- | --- |
| Directory Offset
 | String | The directory offset of the working directory for the current job. Use a period (.) to clone into the 
current working directory. |
| Exclude Filters | String | A list of user names to exclude. |
| File Filters | String | 
Restrict the changelog to files matching these patterns. Start each lines with a plus sign (+) to include or minus sign 
(- )to exclude. You can use the following wildcards in the pattern: *, **, and ?. |
| Populate Locations | String | A 
list of depot-relative path for the files that you want to populate the workspace or stream. The pop command is use to 
restore the listed files.Only the specified files are updated, without building the associated directory tree. |
| 
Repository |  | The AccuRev repository to be used. |
| Revision | String | The version that is to be checked out. |
| 
Stream | String | The stream that is to be checked out. |




