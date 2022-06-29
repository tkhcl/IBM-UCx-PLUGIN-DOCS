
Maven Resolve - Usage
=====================

# Usage


### Usage



The format that is required by the Artifacts field in the [Maven Resolve](#maven_resolve "Maven Resolve step") step is groupId/artifactId/version/filename. The default value of the Artifacts field is ``${p:component/MavenComponentProperties/groupId}``/``${p:component/MavenComponentProperties/artifactId}``/``${p:version.name}``/``${p:component/MavenComponentProperties/artifactId}``-``${p:version.name}``.``${p:component/MavenComponentProperties/extension}``.

You must configure the component properties that are used in the Artifacts field before you run the [Maven Resolve](#maven_resolve "Maven Resolve step") step. To learn more about component properties, see [Component properties](http://www-01.ibm.com/support/knowledgecenter/SS4GSP_6.1.1/com.ibm.udeploy.doc/topics/comp_properties.html "Component properties") in the product help. The default value of the Artifacts field uses the following combination of properties for the file name: ``${p:component/MavenComponentProperties/artifactId}``-``${p:version.name}``.``${p:component/MavenComponentProperties/extension}``.Configure the properties so that the file name matches the file name in the Maven repository.


|Back to ...||Latest Version|Maven Resolve ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[10.1126874](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/Maven/ucd-Maven-10.1126874.zip)|[Readme](README.md)|[Overview](overview.md)|[Steps](steps.md)|[Downloads](downloads.md)|
