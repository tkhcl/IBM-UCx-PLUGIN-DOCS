
IBM DataPower Configuration Manager - Usage
===========================================

# Usage


### Usage




* [Automated DataPower Deployment and Management Using UrbanCode Deploy at HM Health Solutions](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&referrer=&eventid=1457384&sessionid=1&key=B964DE08F3C2EEC28B45B7633953679E&regTag=&sourcepage=register): Webinar on how HighMark Health Solutions uses IBM UrbanCode and DataPower in production. Requires short sign-up to watch.
* [Creating Versions without a Build or CI Tool](https://www.urbancode.com/resource/creating-versions-without-a-build-or-ci-tool/): Import IBM DataPower artifacts with our suggested approach.
* [Import (Basic) Walkthrough](https://www.urbancode.com/2017/08/04/datapower-plugin-basic-import-walkthrough/): Complete beginner walkthrough for IBM UrbanCode and the DataPower plug-in.
* [DataPower Plugin GitHub Wiki](https://github.com/ibm-datapower/datapower-configuration-manager/wiki): Complete documentation on the plugin and DCM command line interface.
* [Definition File Walkthrough](https://www.urbancode.com/2017/08/04/datapower-plugin-definition-file-walkthrough/): Advanced walkthrough of the DataPower plug-in focusing on comprehension of the Definitions file.
* [Docker DataPower Environment](https://developer.ibm.com/datapower/docker/): Simple Docker DataPower environment to get started quickly. In addition to the directions given in the documentation, follow the two steps below to enable the plug-in to communicate with the DataPower service.
+ Add the `-p 5550:5550` argument to the `docker run` command (Step 4).
+ Enable the XML connection via the DataPower cli. After running the Docker container for the first time, immediately after Step 6 run:
- `xml-mgmt 0 5550;`
- `write mem;`
* [Domain Deployment Architecture and Implementation using IBM DataPower and UrbanCode Deploy](https://www.urbancode.com/resource/domain-deployment-architecture-and-implementation-using-ibm-datapower-and-urbancode-deploy/): Best practices around domain deployment implementation and architectural organization using IBM DataPower and UrbanCode Deploy.
* [IBM Datapower GatewaysDevops with UrbanCode Deploy](https://www.slideshare.net/JaredPutman1/ibm-datapower-gateways-devops-with-urbancode-deploy): Slideshow describing the capabilities of IBM UrbanCode Deploy and IBM DataPower Gateways.

|Back to ...||Latest Version|IBM DataPower Configuration Manager ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[9.827594](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/datapower/datapower-9.827594.zip)|[Readme](README.md)|[Overview](overview.md)|[Steps](steps.md)|[Downloads](downloads.md)|
