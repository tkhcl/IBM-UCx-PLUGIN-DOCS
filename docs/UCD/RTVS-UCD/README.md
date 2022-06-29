
IBM Rational Test Virtualization Server (RTVS)
==============================================

The Green Hat plug-in for UrbanCode Deploy that was shipped earlier has been split into the following two parts in the current release:

* [IBM Rational Integration Tester (RIT) plug-in](https://www.urbancode.com/plugin/ibm-rational-integration-tester-rit/), which helps you initiate integration tests from UrbanCode Deploy server.
* Service virtualization plug-in, which executes virtual services that model services which your application depends on. You can initiate the execution of virtual services from UrbanCode Deploy server.

All the three plug-ins (Green Hat plug-in, Rational Integration Tester plug-in, and the Service Virtualization plug-in) can coexist on the same UrbanCode Deploy server. All the process steps supported by the individual plug-ins are still functional.

The steps in the Service Virtualization plug-in use the Rational Test Control Panel Ant client to communicate with the server.

**Platform Support**
* This plug-in runs on all operating systems that are supported by both the IBM UrbanCode Deploy agent (except for z/OS) and the Rational Test Control Panel Ant client
* This plug-in works with Rational Test Workbench v8.5 or higher.




**Known Limitations**



The [Start scenario](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#start_scenario) and [Stop scenario](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#stop_scenario) steps do not work within a transient environment.


Available Steps
---------------

[Create a transient environment](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#create_transient_environment)

[Delete a transient environment](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#delete_transient_environment)

[Start a scenario](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#start_scenario)

[Start a stub](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#start_stub)

[Stop a scenario](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#stop_scenario)

[Stop a stub](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#stop_stub)

[Update a transient environment](https://developer.ibm.com/urbancode/plugindoc/ibmucd/sv-ucd/1-1/stepssv/#update_transient_environment)



|Back to ...||Latest Version|||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[4.0](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/RTVS-UCD/RTVS-UCD-4.0.zip)|[Overview](overview.md)|[Usage](usage.md)|[Steps](steps.md)|[Downloads](downloads.md)|
