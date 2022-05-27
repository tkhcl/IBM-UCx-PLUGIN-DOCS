
ClearCase Base Snapshot - Documentation
=======================================

# Overview




### Overview




 


IBM Rational ClearCase allows you to manage source files and software build history for your 
organization. 


The ClearCase Base Snapshot plug-in integrates IBM UrbanCode Build with IBM Rational ClearCase allowing
 source to be pulled from the ClearCase repository for builds. This plug-in provides integration if you are not using 
the unified change management (UCM) process. If using UCM, see [ClearCase UCM plug-
in](https://www.urbancode.com/plugin/clearcase-ucm/).


### Compatibility



This plug-in requires IBM UrbanCode Build 
version 6.1 and later.


The plug-in runs on any agents that the IBM UrbanCode Build server supports.


### Installation



No special steps are required for installation. See [Installing plug-ins in 
UrbanCode](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in 
UrbanCode").




# Usage




### Usage




 



The IBM UrbanCode Build ClearCase Base Snapshot plug-in provides integration properties,that define
 the connection between the UrbanCode Build server and Rational ClearCase server. For details, see 
[Repositories](http://www.ibm.com/support/knowledgecenter/SS8NMD_6.1.2/com.ibm.ucbuild.doc/topics/settings_project_repo_cpt.html).
 The integration automates populating a ClearCase workspace, creating a label, and publishing source changes to the 
Changes tab of the build life.




The repository is configured based on a workflow.




# Steps




### Steps




 



Process steps in the ClearCase Base Snapshot plug-in

----------------------------------------------------


* [ClearCase Changelog](#clearcase_changelog)
* [ClearCase 
Cleanup](#clearcase_cleanup)
* [ClearCase Get Source](#clearcase_get_source)
* [ClearCase Label](#clearcase_label)
* 
[ClearCase Quiet Period](#clearcase_quiet_period)




ClearCase Changelog
-------------------


Perform a ClearCase 
changelog.




*Input properties for the ClearCase Changelog step*  | Name | Type | Description | Required |
| Changes 
URL | String |  | No |
| End Date | String | End the changelog at this date (‘yyyy-MM-dd HH:mm:ss z’ OR
‘E MMM dd 
HH:mm:ss zzz yyyy’ OR milliseconds since Unix Epoch) | No |
| End Revision | String | End the changelog at this revision
 | No |
| Source Config |  |  | No |
| Start Date | String | Start the changelog at this date (‘yyyy-MM-dd HH:mm:ss z’ 
OR
‘E MMM dd HH:mm:ss zzz yyyy’ OR milliseconds since Unix Epoch) | No |
| Start Revision | String | Start the changelog
 at this revision | No |


ClearCase Cleanup
-----------------


Perform a cleanup of the ClearCase working directory.





*Input properties for the ClearCase Cleanup step*  | Name | Type | Description | Required |
| Source Config |  |  |
 No |


ClearCase Get Source
--------------------


This is a no-op.




*Input properties for the ClearCase Get Source 
step*  | Name | Type | Description | Required |
| Date | String | Date of source code to checkout (‘yyyy-MM-dd HH:mm:ss 
z’ OR ‘E MMM dd HH:mm:ss zzz
yyyy’ OR milliseconds since Unix Epoch). Defaults to
the current time. | No |
| Source 
Config |  |  | No |


ClearCase Label
---------------


ClearCase Label Step.




*Input properties for the ClearCase 
Label step*  | Name | Type | Description | Required |
| Message | String | A message for the label | Yes |
| Source 
Config |  |  | No |
| Tag | String | The label name to create | Yes |


ClearCase Quiet Period
----------------------



Check ClearCase history for quiet period detection and publish the results.




*Input properties for the ClearCase 
Quiet Period step*  | Name | Type | Description | Required |
| End Date | String | End the changelog at this date 
(‘yyyy-MM-dd HH:mm:ss z’ OR
‘E MMM dd HH:mm:ss zzz yyyy’ OR milliseconds since Unix Epoch) | No |
| Source Config |  |  
| No |
| Start Date | String | Start the changelog at this date (‘yyyy-MM-dd HH:mm:ss z’ OR
‘E MMM dd HH:mm:ss zzz yyyy’
 OR milliseconds since Unix Epoch) | No |




# Settings




### Settings




 



The following settings are available when you import component versions by using the ClearCase 
Base Snapshot plug-in.



* [ClearCase Base Snapshot Repository](#clearcase_base_snapshot_repository_role)
* [ClearCase 
Base Snapshot Source Config](#clearcase_base_snapshot_source_config_role)


### ClearCase Base Snapshot Repository





*Properties for the ClearCase Base Snapshot Repository role*  | Name | Type | Description |
| --- | --- | --- |
| 
Command Path | String | The fully qualified path of the cleartool executable file. If specified on the PATH statement, 
this property is not required.  |


### ClearCase Base Snapshot Source Config




*Properties for the ClearCase Base 
Snapshot Source Config role*  | Name | Type | Description |
| --- | --- | --- |
| Changelog Rules | String | The rules 
from the config spec in the following format: vob-name:path:branch:label. Each individual segment may be parameterized. 
|
| Check New Config Spec | Boolean | If enabled, compare a new config spec with a user specified config spec. This 
option allows you to determine if the setcs command was successful, based on the new config spec set on the view rather 
than the outcome of the setcs command.
 |
| Config Spec | String | 
The config spec to be used for the new view. Replace
 any label used in the config spec with a token. For example: replace `/main/LATEST becomes 
/main/$%LATEST%$/main/test/1.0.3` with `/main/test/$%1.0.3%$`. Place a time token after each element rules that does not
 load from a particular label, for example:
`element* /main/LATEST` should become `element* /main/LATEST $[time.token]`

 `element * /main/test/LATEST` should become `element * /main/test/LATEST $[time.token]`
 `element * /main/test/1.0.3` 
should not get a time token. |
| Create Global Labels | Boolean | 
Enable for all labels to be created global. You can 
specify the versioned object bases (VOB) to create the labels within. If you do not specify any VOBs, the load rules are
 used to determine all VOBs that are used and the labels are created in those VOBs. |
| Create Label in VOBs | String | 
A list of of the VOBs where the global labels are created. List each VOB on a separate line. If you are not creating 
global labels, list all the VOBs used in your config spec or leave the field empty and the load the rules are used to 
determine where the labels need to be created in order to complete the labeling process successfully. |
| Delete View 
Private Files During Cleanup | Boolean | Enable for the server to detect and delete any view-private files in the local 
view.Do not enable this feature if the build script handles cleanup of the view. Only the paths specified in the load 
rules are checked for view-private files. |
| Exclude Filters | String | Exclude this list of usernames |
| Fail If No 
Version Selected | Boolean | If enable the populate step fails when a file cannot be found because no version was 
selected in the configuration specification. **Note:** If this is set to false and a file cannot be found, the label 
step might fail. |
| File Filters | String | Restrict the changelog to files matching the specified patterns. Start each
 line with a plus sign (+) to include or a minus sign (-) to exclude files matching the patterns. You can use asterick 
(*), double-asterick (**), and question mark (?) as wildcards in the pattern. |
| Global Storage Path (gpath) | String |
 The value for the -gpath parameter on the mkview command. The value is passed to the command exactly as specified, the 
viewname is not appended to the value. This property is required, ifhostname is specified. |
| Host Storage Path (hpath)
 | String | The value for the -hpath parameter on the mkview command. The specified value is passed to the command 
exactly as specified, the viewname is not appended. This property is required, if hostname is specified. |
| Hostname | 
String | The value for the -host parameter to be used on the mkview command. |
| No-checkout | Boolean | Enable to pass 
the -nco flag to the quietperiod lshistory call. |
| Repository |  | The name of the ClearCase Repository. |
| Tmode | 
Enumeration
 | The Tmode to use. This property is required, if using a Populate step. |
| Use Tags | Boolean | Enable to
 create the view as global. This option can cause problems with creating and dropping snapshots, if the same snapshot is
 on multiple agents. |
| Use VOB Time | Boolean |  |
| VOB Tag Root | String | Specify the VOB tag root. Do not specify 
starting or trailing slashes. Specify this property if you are running cross-platform builds including Windows and Unix 
and using multi-component VOBs. The value is usually `vobs`. |
| View Location | String | If strategy is Already Exists,
 the location of the view is on the local machine. Otherwise, the location of the view storage directory on the 
ClearCase server where the views are stored. For Windows operating systems, the value is always a UNC path. |
| View 
Name | String | The name to use for the view when creating and deleting. Each agent must have a unique view name. You 
can specify a script as the value. For example,  
```${gvy:ProjectLookup.getCurrent().getName()}``_view_``${gvy:AgentHelper.getCurrent().getName()}```. |
| View Strategy 
| Enumeration
 | The view strategy to use. Specify one of the following:
Every Time to create a new view every time 
there is a build
Doesnt Exist to create a new view only if one does not exist already
Already Exists to not create a new
 view |




