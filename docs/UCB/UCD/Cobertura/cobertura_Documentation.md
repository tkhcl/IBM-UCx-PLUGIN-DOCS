
Cobertura - Documentation
=========================

# Overview




### Overview




 


Cobertura is a code coverage tool for software testing. It is a Java tool used to identify which 
parts of your Java program are lacking test coverage. It is based on jcoverage a Java code coverage utility.


Use the 
Cobertura plug-in uploads Cobertura report results as part of the build process.


This plug-in includes one step:


* 
[Publish Cobertura Report](#publish_cobertura_report)



### Step palette


To access this plug-in in the palette, click
 **Quality** > **Code Coverage** > **Cobertura**.


### Compatibility


The steps in this plug-in run on all supported 
platforms.


### Installation


No special steps are required for installation. See [Installing plug-ins in 
UrbanCode](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in 
UrbanCode").


### History


#### Version 5.752901 released on March 9, 2016


Version 5.752901 includes the following 
features and fixes:


* Added RPX dependency.


#### Version 4.604292


Version 4.604292 includes the following features
 and fixes:


Fixed a communication issue that causes the UrbanCode Build server to fail if it is running with an IBM 
JDK or JRE.




#### Version 3.542772


Version 3.542772 includes the following features and fixes:


* Update to a 
newer library version for HTTP communication.


# Steps




### Steps




 



### Process steps in the Cobertura plug-in


* [Publish Cobertura 
Report](#publish_cobertura_report)




### Publish Cobertura Report


Use this step to upload a Cobertura report.





*Input properties for the Publish Cobertura Report step*  | Name | Type | Description | Required |
| --- | --- | --- | 
--- |
| JAVA\_OPTS Variable Name | String | The name of the JAVA\_OPTS environment variable to increase memory. Some 
Cobertura XML reports are large and require increased memory to upload. | No |
| Report Directory | String | The 
directory where the `coverage.xml` file is located. | No |
| Report Name | String | The name of the report to publish. |
 No |




