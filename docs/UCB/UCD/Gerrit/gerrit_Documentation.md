
Gerrit - Documentation
======================

# Overview




### Overview




 


### Overview


Gerrit makes reviews easier by showing changes in a side-by-side display, and 
allowing inline comments to be added by any reviewer.


This plugin provides a step to apply a Gerrit code review.


###
 Compatibility


The steps in this plug-in run on all supported platforms.


### Installation


No special steps are 
required for installation. See [Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").




# Steps




### Steps




 



### Process steps in the Gerrit plug-in


* [Gerrit Review](#gerrit_review)




### Gerrit Review



Apply a Gerrit review.




*Input properties for the  

Gerrit Review step*  | Name | Type | Description | Required |

| --- | --- | --- | --- |
| Commit | String | The commit in Gerrit that is being reviewed. When using this plugin with

Git repository triggers, the value will be in the buildlife/revision property. | No |
| Labels | String | A comma-
separated list of NAME=VALUE pairs | No |
| Message | String |  | No |
| Repo URL | String | The repo URL for the Gerrit
 project. Ex: ssh://user@yourcompany.gerrit.com:29418/path/to/repo.git.
When using this plugin with Git repository 
triggers, the value should be in the buildlife/repo
property. | No |
| Review | Enumeration:
 | The review level to 
apply | No |
| Submit | Boolean | Attempt to submit the patchset | No |




