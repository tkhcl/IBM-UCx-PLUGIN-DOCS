
FindBugs - Documentation
========================

# Overview




### Overview




 


### Overview


The FindBugs plugin uploads the FindBugs results generated during the build to the
 Analytics tab of the BuildLife.


### Compatibility


The steps in this plug-in run on all supported platforms.


### 
Installation


No special steps are required for installation. See [Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").




# Steps




### Steps




 



### Process steps in the FindBugs plug-in


* [Publish Results](#publish_results)




### Publish 
Results


Publish FindBugs results to a build life. This reads the XML output of FindBugs.




*Input properties for the
  

Publish Results step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Exclude Patterns | 
String | Patterns for excluded files from the report, one per line. Files matching these
patterns are unconditionally 
exluded from the report. Patterns can include ?, *, or
**. | No |
| Include Description | Boolean | Include a 
description with each FindBugs finding. Results will be generated
with an output type of xml:withMessages. This is 
optional because it
may consume large amounts of space in the database. | No |
| Include Patterns | String | Patterns 
for including FindBugs XML in the report, one per line. Patterns can include
?, *, or **. | Yes |
| Only Summary Counts 
| Boolean | Only publish the counts of findings to the report and not individual finding details. | No |
| Report Name |
 String | The name of the report published to the build life | Yes |




