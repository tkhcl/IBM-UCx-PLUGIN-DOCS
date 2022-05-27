
Artifactory for IBM UrbanCode Build - Documentation
===================================================

# Overview




### Overview




 


### Compatibility


The IBM UrbanCode Build automation plug-in for Artifactory works with 
Artifactory version 4. The Artifactory Pro edition is also supported. This plug-in requires version 6.1.2 or later of 
IBM UrbanCode Build. This plug-in is supported to run on all operating systems that are supported by the IBM UrbanCode 
Build agent.


### Installation


No special steps are required for installation.




# Steps




### Steps




 



### Process steps in the Artifactory plug-in


* [Download From 
Repository](#download_from_repository)
* [Upload Build Information](#upload_build_information)
* [Upload To 
Repository](#upload_to_repository)




### Download From Repository


Download artifacts from an Artifactory repository





*Input properties for the Download From Repository step*  | Name | Type | Description | Required |
| --- | --- | 
--- | --- |
| Artifactory |  | Select an Artifactory repository from the list or specify a property whose value is
the 
property sheet UUID of the relevant integration. | Yes |
| Repository name | String | The name of the repository. | Yes 
|
| Target Paths | String | A list of target paths to download. Specify each target path in a separate line. Target
path
 should not contain the repository name. | Yes |
| Verify Hash | Boolean | Verify hash value after each artifact 
download is completed. | No |


### Upload Build Information


Upload artifacts to an Artifactory repository




*Input 
properties for the Upload Build Information step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| 
Artifactory |  |  | Yes |
| Build Info Json File | String | Specify the build info json file containing the build 
information to be uploaded | Yes |


### Upload To Repository


Upload artifacts to an Artifactory repository




*Input
 properties for the Upload To Repository step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| 
Artifact Properties | String | Properties to add to each artifact. Properties should be in key=value format in each
line
 | No |
| Artifactory |  | Select an Artifactory repository from the list or specify a property whose value is
the 
property sheet UUID of the relevant integration. | Yes |
| Exclude Patterns | String | List of files to exclude Multiple
 ant-style patterns can be used, with each pattern
in a separate line. | No |
| Include Patterns | String | List of 
files to include. Multiple ant-style patterns can be used, with each pattern
in a separate line. | No |
| Preserve 
Artifact Directories | Boolean | If this checkbox is checked, the directory structure of the included artifacts (based

off of the specified Base Directory property) will be appended to Target Path to determine
each artifacts final target 
path. Otherwise, the final target path will be calculated
based on Target Path and included artifacts file names. | No |

| Repository name | String | The name of the repository. | Yes |
| Target Path | String | The target path of the 
artifacts in Artifactory. | No |




### Roles in the Artifactory plug-in


The plug-in adds these roles automatically 
to resources. You cannot add these roles manually.



* [Artifactory](#artifactory_role)



### Artifactory





*Properties for the Artifactory role*  | Name | Type | Description |
| --- | --- | --- |
| User name | String | The user
 name to use to log in to the Artifactory repository. |
| Password | Password | The password to use to log in to 
Artifactory repository. |
| Artifactory Url | String | The fully-qualified base URL of the Artifactory repository. For 
example: http://192.168.1.1:8081/artifactory. |
| Password Script | String | The property script to use instead of the 
Password property to connect to the Artifactory
repository. If using this property, do not specify a value for the 
Password property. |




