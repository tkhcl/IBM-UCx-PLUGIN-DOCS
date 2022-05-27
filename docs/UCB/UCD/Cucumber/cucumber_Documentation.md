
Cucumber - Documentation
========================

# Overview




### Overview




 


The Cucumber plug-in automates running Cucumber test scenarios. Test scenarios are based on 
Behavior Driven Development (BDD) written to test product features. 


Cucumber test scenarios are written using the 
Gherkin syntax. Each scenario contains a set of steps that are verified processed by the Cucumber tool. A report of 
success or failure is generated for each scenario. Scenarios are stored as `.feature` text files. Step Definitions, 
referred to as *glue* contain a Java method linking to one or more scenario steps.


The Cucumber plug-in contains two 
step that use the Cucumber command line interface to compile step definitions and run test scenarios.


This plug-in 
included the following steps: 


* [Compile step definition](Steps/#compile_step_definition)
* [Run 
Testing](Steps/#run_testing)



### Step palette


To access this plug-in in the palette, click **Quality** > **Unit 
Testing** > **Cucumber**.


### Compatibility


This plug-in requires version 6.1.2 or later of IBM UrbanCode Build. 



This plug-in is supported to run on all operating systems that are supported by the IBM UrbanCode Build agent.


### 
Installation


No special steps are required for installation. See [Installing plug-ins in 
UrbanCode](https://www.urbancode.com/resource/installing-plug-ins-in-urbancode-products/ "Installing plug-ins in 
UrbanCode").


### History


#### Version 1


* Initial release.


# Steps




### Steps




 



### Process steps in the Cucumber plug-in


* [Compile Step Definition](#compile_step_definition)
*
 [Run Testing](#run_testing)




### Compile Step Definition


Compile the step definitions.




*Input properties for 
the Compile Step Definition step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |
| Classpath 
Include | String | The directories to include. Use the double-astrick(**) to include all directories
and the astrick(*) 
to include all files. For example, the pattern dist/**/*.jar would
retrieve the all JAR files. | No |
| Implementation 
Base | String | The implementation base directory, for example:/opt/myProjectName/src/. | No |
| Implementation Include 
| String | List of implementation files to include. Use the double-astrick(**) to indicate include
all directories and 
the astrick(*) to include all files. For example, the pattern
dist/**/*.java retrieves the all JAVA files. | No |
| 
JAVA\_HOME | String | The fully-qualified path to the Java installation for the javac compiler. The default
is the value
 specified in the JAVA\_HOME environment variable of the agent. | No |
| Java ClassPath Base | String | The base 
directory of the Java class path, for example: /jars/. | No |
| Step Definitions Base | String | The bases directory of 
the step definitions. For example, /opt/step\_definitions/. | Yes |
| Step Definitions Include | String | The step 
definitions to include. Use the double-astrick(**) to include all directories
and the astrick(*) to include all files. 
For example, the pattern dist/**/*.java retrieves
the all JAVA files. | Yes |


### Run Testing


Run the test 
scenarios.




*Input properties for the Run Testing step*  | Name | Type | Description | Required |
| --- | --- | --- |
 --- |
| Dry-run | Boolean | Skip execution of the Glue code. | No |
| Features | String | The directory containing the 
feature files. Feature files contain the test scenarios. | Yes |
| JAVA\_HOME | String | The fully-qualified path to the
 Java installation. The default is the value specified
in the JAVA\_HOME environment variable for the agent. | No |
| 
Java ClassPath | String | The directory of the Java classpath, such as: /jars/. | No |
| Name Regexp | String | Run test
 scenarios with the name that matches REGEXP. | No |
| Plugin Type | String | A reporting plug-informat links tags to 
external tools, such as: junit,
html, pretty, progress, json, usage, and rerun. Built-in plug-ins include 
default\_summary
andnull\_summary. Third-party plug-ins can also be included by specifying
thefully qualified class name
 of the plug-in. The default value is pretty. | No |
| Step Definitions | String | The directory containing the step 
definitions. | Yes |
| Strict | Boolean | Undefined and pending steps are treated as errors. | No |
| Tags | String | 
Run test scenarios with the same tag as TAG\_EXPRESSION. | No |




