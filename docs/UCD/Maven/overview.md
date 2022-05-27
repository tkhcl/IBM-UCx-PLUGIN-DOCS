
Maven Resolve - Overview
========================

# Overview



### Overview





The Maven Resolve plug-in includes a step that resolves artifacts from a Maven repository:


* [Maven
 Resolve](#maven_resolve "Maven Resolve")


You can use the Maven Resolve plug-in if you already have a Maven repository
 in use as the definitive source for artifacts. In this scenario, your build automation tool stores new builds in the 
Maven repository and creates a corresponding empty component version in IBM UrbanCode Deploy, where the name of the 
component version matches the Maven identifier. Then, instead of using the Download Artifacts step, you use the Maven 
Resolve plug-in to retrieve the artifacts from the Maven repository and deploy them on the agent computer.


To add the 
Maven Resolve plug-in steps to processes, click **Repositories > Artifact > Maven** in the step palette of the process 
editor.


To use a Maven repository with the Codestation repository in IBM UrbanCode Deploy, see the [Maven source 
configuration plug-in](https://www.urbancode.com/plugin/maven-ibmucd/).


### Compatibility


This plug-in requires 
version 6.0.1 or later of IBM UrbanCode Deploy.


### Installation


No special steps are required for installation. See
 [Installing plug-ins in UrbanCode Deploy](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/
 "Installing plug-ins in UrbanCode Deploy").


### History


#### Version 10


Log4j issue addressed.


#### Version 9



Fixes APAR PI98904 Support resolving Maven snapshot versions using hidden property. Function requires Maven Source 
Config plug-in version 13+.


#### Version 8


Support property file encryption.


#### Version 7


Update Maven resolve
 step to split artifacts properly.


#### Version 6


Version 6 includes a fix for APAR PI50033 related to cleaning up 
temporary files.


#### Version 2


Version 2 of the plug-in points to component source configuration by default.


####
 Version 1


Version 1 is the initial release of the plug-in.




|Back to ...||Latest Version|Maven Resolve ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[10.1126874](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/Maven/ucd-Maven-10.1126874.zip)|[Readme](README.md)|[Usage](usage.md)|[Steps](steps.md)|[Downloads](downloads.md)|
