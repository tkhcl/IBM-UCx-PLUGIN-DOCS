
GitHub - Overview
=================

# Overview



### Overview



 The GitHub plug-in provides for integration with a GitHub server. This plug-in imports issues, pull 
request and commit data from a GitHub server and saves them as UrbanCode Velocity issues. Data between the GitHub server
 and the UrbanCode Velocity server is synchronized every five minutes.
Compatibility
-------------


Must be running 
UrbanCode Velocity version 1.2.1 and later to use the plug-in.


**Note:** For integrations created before upgrading to 
version 2.4.0 of UrbanCode Velocity, Auto-generated User Access Key is not present, so the integration will fail after 
upgrading. In this case, you have to manually add a new User Access Key in the hidden property named ***UrbanCode 
Velocity User Access Key.***


Upgrade impact
--------------


When migrating to version 1.0.30 of this plug-in, you 
must make an update to your integration. The **Name** property has been removed. Use the Repositories property to 
identify one or more GitHub repositories to be used to import data. Additionally, you must specify a value for the 
**UrbanCode Velocity User Access Key** property.


Versions
--------


UrbanCode Velocity plug-in images are located in 
DockerHub. To view available versions, see the [UrbanCode DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-
github/tags).


History
-------


### Version 1.1.18


* ReSync support added (support starts with UrbanCode Velocity 
version 2.4.4 or later).
* Auto-generated User Access Key support added (support starts with UrbanCode Velocity version 
2.4.0 or later).


### Version 1.1.1


* Added support to pull commits from additional branches.


### Version 1.0.49



* Added history to GitHub issues


### Version 1.0.40


* Imports GitHub issues


### Version 1.0.36


* Support Non 
Master Branch Information


### Version 1.0.34


* Added HTTP proxy support


### Version 1.0.32


* Fix for repository 
URL


### Version 1.0.31


* Removed redundant URL field


### Version 1.0.30


* Removed the **Name** property in the 
configuration properties
* Improved logging
* UrbanCode Velocity User Access Key is added as a mandatory field for 
integration


### Version 1.0.29


* Updated to handle a null commit author in the repository


### Version 1.0.28


* 
Update plug-to incorporate bug fixes


### Version 1.0.27


* Update plug-to incorporate bug fixes


### Version 1.0.26



* Update plug-to incorporate bug fixes


### Version 1.0.25


* Update plug-to incorporate bug fixes


### Version 
1.0.24


* Update plug-to incorporate bug fixes


### Version 1.0.23


* Update plugin version from 0.x.x to 1.x.x 
format.


### Version 0.0.21


* Support for multiple repositories


### Version 0.0.11


* Initial release




|Back to ...||Latest Version|GitHub |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[1.3.29]()|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
