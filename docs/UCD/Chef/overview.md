
Chef - Overview
===============

# Overview



### Overview




 


### Overview


Chef is a tool for automating deployment tasks. The Chef plug-in includes a step that installs Chef and a step that uses Chef to install a Chef node on a system.


In the context of Chef automation, a *node* represents a computer system. A Chef node file includes a list of Chef recipes and roles. These recipes and roles point to automated tasks to run on the node.


To use this plug-in, first run the Install Chef step. Then, run the Install Chef Node step to configure the target system according to a Chef node file. You can run this step multiple times on the same target system to apply multiple Chef node files.


### Compatibility


Version 1 of this plug-in requires version 6.0.0 of IBM UrbanCode Deploy.


This plug-in is supported to run on all operating systems that are supported by both the IBM UrbanCode Deploy agent (except for z/OS).


This plug-in is supported to run against Chef v11.6.0-1 or higher.



### Installation


No special steps are required for installation. See [Installing plug-ins in UrbanCode Deploy](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in UrbanCode Deploy").




|Back to ...||Latest Version|Chef ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[3.1056568](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/Chef/Chef-3.1056568.zip)|[Readme](README.md)|[Steps](steps.md)|[Usage](usage.md)|[Downloads](downloads.md)|
