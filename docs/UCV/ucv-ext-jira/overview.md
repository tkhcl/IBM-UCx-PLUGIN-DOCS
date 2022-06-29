
Jira - Overview
===============

# Overview


### Overview


The Jira plug-in provides for integration with a Jira server. This plug-in imports Jira issues and
saves them as UrbanCode Velocity issues. Data between the Jira server and the UrbanCode Velocity server is synchronized
every five minutes.

Compatibility
-------------

Must be running UrbanCode Velocity version 1.2.1 and later to use
the plug-in.

Upgrade notes
-------------

Beginning with UrbanCode Velocity version 2.4.0 users must enter a user
access key is required to connect with the UrbanCode Velocity server. If you are upgrading from a previous version, you
must obtain and add the key to the UrbanCode Velocity configuration property. If the user access key is not added, the
integration fails. A proper JQL query must be provided while integration .

Versions
--------

UrbanCode Velocity
plug-in images are located in DockerHub. To view available versions, see the [UrbanCode
DockerHub](https://hub.docker.com/r/urbancode/ucv-ext-jira/tags).

History
-------


### Version 2.1.1

* Added JQL
Query.
* Removed Project Keys.
* Removed Initial Sync Date.

### Version 1.1.89

* Labels updated.
* Debug logs added.

* Reintroduce base path.
* Initial Sync Data added.
* Payload size more than 10MB data issue resolved.

### Version
1.0.80

* Minor enhancements.

### Version 1.0.74

* Minor enhancements.

### Version 1.0.65

* Minor enhancements.


### Version 1.0.64

* ReSync support added. Applies to UrbanCode Velocity version 2.4.4 or later.
* Auto-generated
User Access Key support added. Applies to UrbanCode Velocity version 2.4.0 or later.

### Version 1.0.51

* Minor
enhancements.

### Version 1.0.50

* Jira rate limit issue fix.

### Version 1.0.49

* Minor bug fix.

### Version
1.0.39

* Minor bug fix.

### Version 1.0.38

* Minor bug fix.

### Version 1.0.36

* Added HTTP proxy support.


### Version 1.0.27

* Update plugin version from 0.x.x to 1.x.x format.

### Version 0.0.17

* Initial release


|Back to ...||Latest Version|Jira |||
| :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Velocity Plugins](../README.md)|[2.2.1](https://raw.githubusercontent.com/UrbanCode/IBM-UCV-PLUGINS/main/files/ucv-ext-jira/ucv-ext-jira-2.2.1.tar.zip)|[Readme](README.md)|[Usage](usage.md)|[Downloads](downloads.md)|
