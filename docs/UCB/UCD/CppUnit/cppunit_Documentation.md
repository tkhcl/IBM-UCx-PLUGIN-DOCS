
CppUnit - Documentation
=======================

# Overview




### Overview




 



### Overview


Publish CppUnit results as a Report within UrbanCode Build


### Compatibility



The steps in this plug-in run on all supported platforms.


### Installation


No special steps are required for 
installation. See [Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.0/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").




# Steps




### Steps




 



### Process steps in the CppUnit plug-in


* [CppUnit Report](#cppunit_report)




### CppUnit 
Report


Publish CppUnit results as a Report




*Input properties for the  

CppUnit Report step*  | Name | Type | 
Description | Required |
| --- | --- | --- | --- |
| Exclude Patterns | String | Patterns for excluded files from the 
report, one per line. Files matching these
patterns are unconditionally excluded from the report. Patterns can include 
?, *,
or **. | No |
| Include Patterns | String | Patterns for including CppUnit XML in the report, one per line. 
Patterns can include
?, *, or **. | Yes |
| Report Name | String | The name for this report | No |
| Source Directory | 
String | Please specify the Base Directory | Yes |




