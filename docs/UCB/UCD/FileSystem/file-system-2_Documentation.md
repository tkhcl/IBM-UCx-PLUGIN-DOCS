
File System for IBM UrbanCode Build - Documentation
===================================================

# Overview




### Overview




 


Use the File System plug-in to work with a repository where files are stored in the working 
directory.


### Compatibility


The steps in this plug-in run on all supported platforms.


### Installation


No 
special steps are required for installation. See [Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").


### History


#### Version 4


This version of the plug-in includes 
translated steps and properties.


#### Version 3


This version of the plug-in includes a fix for an issue where 
communication with the IBM UrbanCode Build server would fail when using an IBM JDK or JRE.




# Steps




### Steps




 



### Process steps in the File System plug-in


* [FileSystem Changelog](#filesystem_changelog)
* 
[FileSystem Checkout](#filesystem_checkout)
* [FileSystem Cleanup](#filesystem_cleanup)
* [FileSystem Quiet 
Period](#filesystem_quiet_period)
* [FileSystem Tag](#filesystem_tag)




### FileSystem Changelog


Get the latest 
modified date for the working directory




*Input properties for the  

FileSystem Changelog step*  | Name | Type | 
Description | Required |
| --- | --- | --- | --- |
| Changes URL | String |  | No |
| End Date | String | End the 
changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |
| 
Source Config |  |  | No |
| Start Date | String | Start the changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd 
HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |


### FileSystem Checkout


Does nothing.




*Input 
properties for the  

FileSystem Checkout step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| 
Source Config |  |  | No |


### FileSystem Cleanup


Perform a cleanup of the working directory




*Input properties 
for the  

FileSystem Cleanup step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Source Config 
|  |  | No |


### FileSystem Quiet Period


Get the latest modified date for the working directory




*Input 
properties for the  

FileSystem Quiet Period step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |

| End Date | String | End the changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz yyyy OR 
milliseconds since Unix Epoch) | No |
| Source Config |  |  | No |
| Start Date | String | Start the changelog at this 
date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |


### FileSystem Tag



Does nothing.




*Input properties for the  

FileSystem Tag step*  | Name | Type | Description | Required |
| --- |
 --- | --- | --- |
| Source Config |  |  | No |




### Roles in the File System plug-in


The plug-in adds these roles 
automatically to resources. You cannot add these roles  

manually.



* [FileSystem 
Repository](#filesystem_repository_role)
* [FileSystem Source Config](#filesystem_source_config_role)



### FileSystem 
Repository


Instead of using a SCM system, the File System repository expects files to be present  

in the working 
directory.



### FileSystem Source Config




*Properties for the  

FileSystem Source Config role*  | Name | Type | 
Description |
| --- | --- | --- |
| Directory Offset | String | Directory offset from the current jobs working 
directory. (Use . to clone into
the current working directory) |
| File Filters | String | Restrict changelog to files 
matching these patterns. Lines start with + to include
andto exclude.Wildcards *, **, and ? are allowed. |
| Repository 
|  | Select the File System Repository |




