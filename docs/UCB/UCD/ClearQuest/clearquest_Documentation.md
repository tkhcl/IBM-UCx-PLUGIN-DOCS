
ClearQuest - Documentation
==========================

# Overview




### Overview




 


### Overview


Leverage this integration with ClearQuest to create or update records within 
ClearQuest, and run reports against you change requests.


### Compatibility


The steps in this plug-in run on all 
supported platforms.


### Installation


No special steps are required for installation. See [Installing plug-ins in 
UrbanCode Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html
 "Installing plug-ins in UrbanCode Build").




# Steps




### Steps




 



### Process steps in the ClearQuest plug-in


* [Add Comment](#add_comment)
* [Create 
Defect](#create_defect)
* [Publish Defect Report](#publish_defect_report)
* [Resolve Issue](#resolve_issue)




### Add 
Comment


Add Comments from the current changelog to matching ClearQuest Defects




*Input properties for the  

Add 
Comment step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| ClearQuest Server |  | The 
ClearQuest server. This may be configured under the System tab. | Yes |
| Comment | String | The content of the comment.
 | Yes |
| Defect ID | String | The ID of the defect to place the comment on. | Yes |


### Create Defect


Create a new
 defect in a ClearQuest Defect Tracker




*Input properties for the  

Create Defect step*  | Name | Type | Description
 | Required |
| --- | --- | --- | --- |
| ClearQuest Project Name | String | The name of the project in ClearQuest. | No
 |
| ClearQuest Server |  | The ClearQuest server. This may be configured under the System tab. | Yes |
| Defect 
Description | String | The description of the defect. | No |
| Headline | String | The headline of the defect. | Yes |
|
 Owner | String | The owner of the defect. | No |
| Priority | String | The priority level of the defect. | No |
| 
Severity | String | The severity level of the defect. | Yes |


### Publish Defect Report


Create a Report of 
ClearQuest defects from the current changelog




*Input properties for the  

Publish Defect Report step*  | Name | 
Type | Description | Required |
| --- | --- | --- | --- |
| ClearQuest Server |  | The ClearQuest server. This may be 
configured under the System tab. | Yes |
| Defect ID Pattern | String | This is a regular expression to locate 
ClearQuest-defect ids within
changelog comments.You may add () around the portion of the pattern
which identifies the 
actual Issue ID. The pattern TST-[0-9]+ would match
(returning the same string as issue ids) TST-1 and TST-932415, but 
not
match TST-a, TST-, or TST.1. The pattern Issue:\[(TST-[0-9]+)\]
would match Issue:[TST-1] using issue id TST-1 | Yes
 |


### Resolve Issue


Resolve a ClearQuest Defect




*Input properties for the  

Resolve Issue step*  | Name | Type
 | Description | Required |
| --- | --- | --- | --- |
| ClearQuest Server |  | The ClearQuest server. This may be 
configured under the System tab. | Yes |
| Defect ID | String | The id of the ClearQuest defect. | Yes |
| Resolution | 
String | The resolution which resolved the issue. | No |




### Roles in the ClearQuest plug-in


The plug-in adds 
these roles automatically to resources. You cannot add these roles  

manually.



* [ClearQuest 
Server](#clearquest_server_role)



### ClearQuest Server




*Properties for the  

ClearQuest Server role*  | Name | 
Type | Description |
| --- | --- | --- |
| CQperl.exe path | String | The filepath designating CQperl.exe. |
| Database 
Name | String | The name of the ClearQuest database. |
| Database Schema | String | The ClearQuest database schema name.
 |
| Issue URL | String | This field provides a template which may be used throughout
uBuild to generate links from 
issues directly to an issue description
page within your issue tracker. The value ``${issueId}`` will be replaced
in the
 template with the issue id of the associated issue. Please provide
a url template such as 
http://bugs.company.com/browse/``${issueId}``. |
| Password | Password | The user password. |
| Scripted Password | 
String | If you would prefer to resolve the password with a script,
enter it here. |
| Username | String | The username 
to connect to the ClearQuest database. |




