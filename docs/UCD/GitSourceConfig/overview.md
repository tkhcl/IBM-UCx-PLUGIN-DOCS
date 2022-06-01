
Git - Overview
==============

# Overview



### Overview




 


The Git plug-in automates importing artifacts from a Git repository.


This plug-in includes one step which has no input properties:


* [Import Version](#import_version)


The plug-in adds the following roles to resources:


* [GitComponentProperties](#gitcomponentproperties_role)
* [GitImportProperties](#gitimportproperties_role)



### Step palette


To access this plug-in in the palette, click **Source and Repositories** > **Git**.


### Compatibility


This plug-in requires UrbanCode Deploy version 6.0 or later.


This plug-in supports all versions of the Git client.


This plug-in runs on all operating systems that UrbanCode Deploy supports, except the IBM z/OS operating system.


### Installation


This plug-in is installed when installing IBM UrbanCode Deploy. When new plug-in versions are available, see [Installing plug-ins in UrbanCode Products](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in UrbanCode Deploy") to update the plug-in.


### History


#### Version 15


* APAR PI89045: add support for setting isFinished flag when importing versions


#### Version 14


* Fixes APAR PI87707, a regression where the user who requested a manual version import was not being tracked.


#### Version 13


* Fixes APAR PI94103. Added an option to disable SSL certificate verification.


#### Version 12


* Fixes APAR PI89187. Branch is now specified when making inital git clone command.
* Branch property is now optional. Default value is master.
* Improved error output when unable to identify Commit IDs or Tags.
* If specified revision is not found, a hollow component version will no longer be created.


#### Version 11


* RFE 110682. On default automatic imports where Watch for Tags is not specified, the plug-in will make a shallow copy of depth 1 to save time and space.
* If a Version/Tag value or the Watch for Tags check box is specified, a full clone will be made.


#### Version 10


* RFE 86753. Added support for Git submodules.


#### Version 9


* Fixes APAR PI40551. Now uses working directory for temporary artifact storage.


#### Version 8


* This release now encodes username to fix authentication issues.


#### Version 7


* This release is being provided to include updated translations.


#### Version 6


* Fixes APAR PI63702. Adds functionality to separate Includes and Excludes parameters with new lines or commas.


#### Version 5


* Fixes APAR PI57417. Plug-in now checks the agent settings for acceptance of self signed certificates.


#### Version 4


* Version 4 of this plug-in adds a setting to authenticate with a Git repository.


|Back to ...||Latest Version|Git |||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[23.1131566]()|[Readme](README.md)|[Troubleshooting](troubleshooting.md)|[Settings](settings.md)|[Usage](usage.md)|[Downloads](downloads.md)|
