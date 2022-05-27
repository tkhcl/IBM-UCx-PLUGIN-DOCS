
CA Harvest SCM - Documentation
==============================

# Overview




### Overview




 


CA Harvest Software Change Manager (CA Harvest SCM) manages source files and software build 
history for your organization. It automates the change management lifecycle, source code versioning and streamlines 
workflows.


The plug-in provides integration properties, that define the connection between the UrbanCode Build server 
and a CA Harvest server. The integration automates populating a Harvest workspace and publishing source changes to the 
Changes tab of the build life. For details about repositories in IBM UrbanCode Build, see 
[Repositories](http://www.ibm.com/support/knowledgecenter/SS8NMD_6.1.2/com.ibm.ucbuild.doc/topics/settings_project_repo_cpt.html)
 in the product documentation.


### Compatibility


This plug-in requires IBM UrbanCode Build version 6.1 and later.



The plug-in runs on any agents that the IBM UrbanCode Build server supports.


### Installation


No special steps are 
required for installation. See [Installing plug-ins in UrbanCode](https://www.urbancode.com/resource/installing-plug-
ins-in-urbancode-products/ "Installing plug-ins in UrbanCode").


### History


#### Version 7


Fix APAR PH10867Use 
includeFiles source property in quiet period step.


#### Version 6


Fix changelog parser logic to correctly handle 
empty data columns.


#### Version 5


Version 5 includes the following features and fixes:


* Added RPX dependency.
* 
Translation for step information.


#### Version 4


Version 4 includes the following features and fixes:


* Fixed a 
communication issue where the UrbanCode Build server would fail if it was running with an IBM JDK or JRE.


#### Version
 3


Version 3 includes the following features and fixes:


* Update to a newer version of a library for HTTP 
communication.


# Steps




### Steps




 



### Process steps in the Harvest plug-in


* [Harvest Changelog](#harvest_changelog)
* [Harvest 
Checkout](#harvest_checkout)
* [Harvest Cleanup](#harvest_cleanup)
* [Harvest Quiet Period](#harvest_quiet_period)





### Harvest Changelog


Perform a Harvest changelog and publish the results.




*Input properties for the Harvest 
Changelog step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Changes URL | String |  | No |
| 
End Date | String | End changelog at this date. Will check the beginning of
dd, so if you want the full day included add
 one day (mm/dd/yyy) | No |
| Source Config |  |  | No |
| Start Date | String | Start changelog at this date. Will 
check the beginning
of dd, so if you want the full day included add one day (mm/dd/yyy) | No |


### Harvest Checkout



Perform a Harvest checkout of the workflows source




*Input properties for the Harvest Checkout step*  | Name | Type |
 Description | Required |
| --- | --- | --- | --- |
| Clean Workspace | Boolean | Erase all files from the workspace 
before performing checkout | No |
| Date | String | Date of sourcecode to checkout (yyyy-MM-dd HH:mm:ss z OR
E MMM dd 
HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch). Defaults to the current
time. | No |
| Source Config |  |  | No |



### Harvest Cleanup


Perform a cleanup of the Harvest working directory




*Input properties for the Harvest 
Cleanup step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Source Config |  |  | No |


### 
Harvest Quiet Period


Perform a Harvest changelog for quiet period detection and publish most recent change  

date 
within the period.





*Input properties for the Harvest Quiet Period step*  | Name | Type | Description | Required |
|
 --- | --- | --- | --- |
| End Date | String | End changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss 
zzz yyyy OR milliseconds since Unix Epoch) | No |
| Source Config |  |  | No |
| Start Date | String | Start changelog 
at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |




### Roles
 in the Harvest plug-in


The plug-in adds these roles automatically to resources. You cannot add these roles  


manually.



* [Harvest Repository](#harvest_repository_role)
* [Harvest Source Repo](#harvest_source_repo_role)



### 
Harvest Repository


Global settings for accessing Harvest repositories.




*Properties for the Harvest Repository 
role*  | Name | Type | Description |
| --- | --- | --- |
| Command Path | String | The directory that contains all of 
the Harvest command line interface (CLI) commands.
For example: /opt/CA/scm/bin. Specify this property only when
the 
command is not on the path. |
| Harvest Broker | String | The Harvest broker to run CLI commands against. |
| Password 
Script | String | A script or property lookup for the password. If using this property, do not specify
a value for the 
Password property. |
| Repository Password | Password | The password to use for access to Harvest repositories |
| 
Repository Username | String | The username to use for access to Harvest repositories |


### Harvest Source Repo





*Properties for the Harvest Source Repo role*  | Name | Type | Description |
| --- | --- | --- |
| Checkout Includes | 
String | Files included for the checkout command. Wildcards are allowed. For example specify
*.js to include all .js 
files. |
| Checkout Method | Enumeration:
 | The method used to checkout files. All methods with the exception of browse
 requires
a package.Update:Copy items and reserve them for check
in.Browse:Copy items but do not reserve them to be

checked back in.Reserve Only:Do not copy any data but
marks items as reserved to be checked back in.Synchronize:

Identify the versions of the files on the client using the signature file.
Concurrent Update: Copy items and reserve 
them for check in. The reserved version
is created on a branch. |
| Directory Offset | String | The directory offset 
from the current jobs working directory. Use a period (.) to
clone intothe current working directory. |
| Exclude 
Filters | String | A list of usernames to exclude. |
| File Filters | String | Restrict the changelog to the files 
matching the specified patterns. Specify each
pattern on a new line.Start each line with a plus sign
(+) to include or a
 minus sign (-) to exclude files matching the patterns.
You can use asterick (*), double-asterick (**), and question 
mark (?) as wildcards
in the pattern. |
| Package | String | The name of the package. |
| Project | String | The project
 where all of your files exist. |
| Recursive Search | Boolean | Recursively search through and select all versions from
 directories below the specified
view path. |
| Repository |  | The Harvest repository to be accessed. |
| Snapshot | 
String | The name of the snapshot view. The state specified must have Snapshot Views enabled. |
| State | String | The 
state in which the user is running the project. For example: Dev. |
| View Path | String | The path to the Harvest 
repository in the Harvest server. For example: \TestRepo. |




