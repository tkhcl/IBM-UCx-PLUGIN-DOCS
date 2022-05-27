
Ant - Documentation
===================

# Overview




### Overview




 


The Ant plug-in is an automation plug-in. You can use the Ant plug-in during deployment to 
automate Ant tasks that are defined in a build.xml file.


### Compatibility


This plug-in requires IBM UrbanCode Build
 version 6.1 or later.


The steps in this plug-in run on all supported platforms.


### Installation


No special steps
 are required for installation. See [Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.1/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").


### History


#### Version 7


This version includes translated steps and 
properties.


#### Version 6


The JVM Properties field was removed.




# Steps




### Steps




 



### Process steps in the Ant plug-in


* [Ant](#ant)




### Ant


Run an Ant script.




*Input 
properties for the Ant step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| ANT\_HOME | String | 
The path to the Ant installation to use to run the Ant script. By default, the path is the ANT\_HOME environment 
variable on the agent. | Yes |
| ANT\_OPTS | String | Ant-specific arguments, which are used in the ANT\_OPTS 
environment variable. Enter each argument on a new line. For example: -Xmx1024m or -XX:MaxPermSize=512m | No |
| Ant 
Properties | String | Ant-specific arguments, such as -v for verbose output. Enter each argument on a new line. | No |
|
 Ant Script File | String | The name of the Ant script file. | Yes |
| JAVA\_HOME | String | The path to the Java 
installation to use to run Ant. By default, the path is the JAVA\_HOME environment variable on the agent. | Yes |
| 
Properties | String | Properties to pass to Ant. These properties are available by name in the Ant script. Enter each 
argument on a new line in the following format: name=value | No |
| Script Content | String | Optional: Specify the 
content of the Ant script. The content is written to the file specified by the Ant Script File field, and then run. | No
 |
| Targets | String | The names of the targets to run in the Ant script file. If blank, the default target is used. | 
No |




