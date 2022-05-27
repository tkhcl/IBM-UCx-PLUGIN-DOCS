
Git for IBM UrbanCode Build - Documentation
===========================================

# Overview




### Overview





The Git plug-in automates cloning a Git repository, tagging source code, and publishing source code 
changes to the Changes page of the build life.


### Compatibility


The Git source config plugin for UrbanCode Build is
 compatible with version 6.1.3 and above.


Supporting GitHub and BitBucket Server repository trigger events requires 
UrbanCode Build 6.1.4.1 and above.


### Installation


No special steps are required for installation. See [Installing 
plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").


### History


#### Version 27


To fix duplicate committer licenses, we 
made provisions to use email ids instead of author names.


#### Version 26


Added provision to disable Build triggers 
on Draft Pull Request.


#### Version 25


 Ensure the local git repository’s remote url is up to date before performing
 a checkout.


#### Version 24


Properly handle charset when reading the response stream in changelog step.


#### 
Version 23


Ignore BitBucket events related to deleting branches.


#### Version 22


Resolve ``${p:triggeredBranch}`` 
using data provided in the payload of repo:refs\_changed events from BitBucket Server.


#### Version 21


Add ability 
to handle repo:refs\_changed and pr:merged events sent by BitBucket Server.


#### Version 20


Add ability to trigger 
builds in response to repo:push events sent by BitBucket.


#### Version 19


Allow triggering builds for changes in 
arbitrary branches of a GitHub repository.


#### Version 18


Avoid NullPointerException if the HTTP client fails to 
execute and throws an exception before returning the response object.


#### Version 17


Prefer using external web URL 
to construct the target URL in Create GitHub Status step when available.


#### Version 16


Fix incompatibility with 
UCB 6.1.2.x that was introduced in version 14 and prevented triggering builds in response to push events sent by GitHub.



#### Version 15


Fix intermittent IOException stream closed errors.


#### Version 14


Added support for triggering
 pre-flight builds for pull request events sent from GitHub. Requires IBM UCB 6.1.3.1 (patched) or later.


#### Version
 13


Added new step for creating commit statuses in GitHub. Requires IBM UCB 6.1.3.1 (patched) or later.


#### Version
 12


Fixed issue with repository trigger script not resolving parameterized repository base URL.


#### Version 11



Fixed infinite build triggering issue with Github if creating a tag with the same name as an existing branch.


#### 
Version 10


Support property file encryption.


#### Version 9


Improved handling of user credentials embedded in 
repository base URL and repository configuration.


#### Version 8


This release includes translated steps and 
properties.


#### Version 7


This release includes a fix for the triggering script.


#### Version 6


This release 
includes support for triggering builds by using GitHub or GitLab webhooks.




# Steps




### Steps






### Process steps in the Git plug-in


* [Create GitHub Status](#create_github_status)
* [Git 
Changelog](#git_changelog)
* [Git Checkout](#git_checkout)
* [Git Cleanup](#git_cleanup)
* [Git Create 
Tag](#git_create_tag)
* [Git Quiet Period](#git_quiet_period)




### Create GitHub Status


Create a commit status in 
GitHub or GitHub Enterprise.




*Input properties for the Create GitHub Status step*  | Name | Type | Description | 
Required |
| --- | --- | --- | --- |
| Base REST URL | String | The base URL of the REST API e.g. 
https://api.github.com. This value should be left
blank to be automatically inferred from GitHubs webhook data, unless a
 different
URL needs be used. | No |
| Context | String | The service that is providing the status. | No |
| Description
 | String | High level summary of the status update. | No |
| Source Config |  |  | No |
| State | Enumeration: | The 
state of the status. | Yes |


### Git Changelog


Perform a Git changelog and publish the results.




*Input 
properties for the Git Changelog step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Changes URL
 | String |  | No |
| End Date | String | End changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz 
yyyy OR milliseconds since Unix Epoch) | No |
| End Revision | String | End changelog at this revision | No |
| Source 
Config |  |  | No |
| Start Date | String | Start changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz
 yyyy OR milliseconds since Unix Epoch) | No |
| Start Revision | String | Start changelog at this revision | No |


###
 Git Checkout


Perform a Git checkout of the workflows source




*Input properties for the Git Checkout step*  | Name 
| Type | Description | Required |
| --- | --- | --- | --- |
| Clean Workspace | Boolean | Erase all files from the 
workspace before performing checkout | No |
| Date | String | Date of sourcecode to checkout (yyyy-MM-dd HH:mm:ss z OR
E
 MMM dd HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch). Defaults to the current
time. | No |
| Source Config |  |  
| No |


### Git Cleanup


Perform a cleanup of the Git working directory




*Input properties for the Git Cleanup 
step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Source Config |  |  | No |


### Git Create 
Tag


Create a tag in Git of the specified working copy.




*Input properties for the Git Create Tag step*  | Name | 
Type | Description | Required |
| --- | --- | --- | --- |
| Message | String | A message for the commit | Yes |
| Source
 Config |  |  | No |
| Tag | String | The tag name to create | Yes |


### Git Quiet Period


Perform a Git changelog 
for quiet period detection and publish most recent change  

date within the period.




*Input properties for the Git 
Quiet Period step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| End Date | String | End 
changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |
| 
Source Config |  |  | No |
| Start Date | String | Start changelog at this date (yyyy-MM-dd HH:mm:ss z OR
E MMM dd 
HH:mm:ss zzz yyyy OR milliseconds since Unix Epoch) | No |




### Roles in the Git plug-in


The plug-in adds these 
roles automatically to resources. You cannot add these roles  

manually.


* [Git Repository](#git_repository_role)
* 
[Git Source Repo](#git_source_repo_role)



### Git Repository


Global settings for accessing git repositories.





*Properties for the Git Repository role*  | Name | Type | Description |
| --- | --- | --- |
| Command Path | String | 
The location of the Git executable (e.g. /usr/bin/git), if it is not specified in
the PATH. |
| Disable Build on Draft 
PR | Boolean | Skip Build triggers on Draft Pull Requests. |
| Password Script | String | Enter a script or property 
lookup to obtain the password. This field will only be
effective if the Repository Password field is blank. |
| 
Repository Base URL | String | A URL prefix for source configurations to specify a relative path to the git repository.

(e.g. https://git.example.com/repos or ssh://git.example.com/repos) |
| Repository Password | Password | The password to
 use for http(s) access to repositories |
| Repository Username | String | The username to use for http(s) access to 
repositories |
| Use Author Email | Boolean | The plugin will use the committer’s email instead of the author’s name.By 
default, the author name is used. |


### Git Source Repo




*Properties for the Git Source Repo role*  | Name | Type |
 Description |
| --- | --- | --- |
| Branch | String | The remote branch name to check out (defaults to master) |
| 
Directory Offset | String | Directory offset from the current jobs working directory. (Use . to clone into
the current 
working directory) |
| Exclude Filters | String | Exclude this list of usernames |
| File Filters | String | Restrict 
changelog to files matching these patterns. Lines start with + to include
and to exclude. Wildcards *, **, and ? are 
allowed. |
| Remote Name | String | The name to use for the remote (defaults to origin) |
| Remote URL | String | The 
path to the project repository e.g. username/project. The value of Remote URL
will be appended to the repositorys Base 
URL |
| Repository |  | Select the Git Repository |




