
Groovy for IBM UrbanCode Build - Documentation
==============================================

# Overview




### Overview




 


The Groovy plug-in is an automation-type plug-in that provides a step for running user-defined 
Groovy scripts.


### Compatibility


This plug-in requires IBM UrbanCode Build version 6.1 or later.


The steps in 
this plug-in run on all supported platforms.


### Installation


No special steps are required for installation. See 
[Installing plug-ins in UrbanCode 
Build](http://www-01.ibm.com/support/knowledgecenter/#!/SS8NMD_6.1.2/com.ibm.ucbuild.doc/topics/plugin_ch.html 
"Installing plug-ins in UrbanCode Build").


### History


#### Version 7


This version of the plug-in includes 
translated steps and properties.


#### Version 6


This version of the plug-in includes a fix for an issue related to 
running scripts on Microsoft Windows.


#### Version 3


This version of the plug-in includes the ability to run JUnit 
test cases in Groovy steps.




# Steps




### Steps




 



### Process steps in the Groovy plug-in


* [Run Groovy Script](#run_groovy_script)




### Run 
Groovy Script


Run a Groovy script.




*Input properties for the Run Groovy Script step*  | Name | Type | Description 
| Required |
| --- | --- | --- | --- |
| Groovy Home | String | Groovy home directory. Default is the value of the 
GROOVY\_HOME environment variable. | Yes |
| Script | String | Enter the script code to run. A java.util.Properties 
variable for output properties to upload to the server is in the outProps context another variable containing all the 
input properties is in the inProps context. | Yes |




