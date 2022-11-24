
IBM Rational Test Automation Server (RTAS) - Steps
==================================================

# Steps


### Steps




Process steps in the IBM Rational Test Automation Server plug-in:

* [Start a job on IBM Rational Test Automation Server](#start_job)


### Start a job on IBM Rational Test Automation Server

Use this step to start a job on the Rational Test Automation Server.


| Name | Type | Description | Required |
| --- | --- | --- | --- |
| Rational Test Automation Server URL | String | The URL of the Rational Test Automation Server. | Yes |
| Offline Token | Password | User provided offline access token for accessing the Rational Test Automation Server. | Yes |
| Team Space Name | String | Team Space name of the project. | Yes |
| Project Name | String | Project name of the job to run. | Yes |
| Branch Name | String | Branch name of the job to run. Default is master. | No |
| Repository Link | String | Repository link for the job to run. | No |
| File Path | String | The path to the Rational Test Automation Server file. | Yes |
| Datasets | String | Optional. Semicolon (;) delimited list of datasets. A replacement for the job to run. For example, `dataset1:dataset2;dataset3:dataset4` | No |
| Variables | String | Runtime job variables. For example, `name1=value1;name2=value2` | No |
| Labels | String | Comma (,) delimited list of labels for the job to run. | No |
| Secrets Collection Name | String | Secrets collection name for the job to run. | No |
| Environment | String | Environment for the job to run. Only applicable for API tests. | No |
| Custom Trust Store Path | String | Path to the custom trust store including the file name. This trust store must include the certificate of the CA that issued the SSL certificate of your IBM Rational Test Automation Server instance or the SSL certificate of your IBM Rational Test Automation Server instance. This field cannot be left blank when the SSL certificate of your IBM Rational Test Automation Server instance is signed by an internal CA or when you're unable to establish secure connection to your IBM Rational Test Automation Server instance. In other cases, it can be left blank. | No |
| Custom Trust Store Password | Password | Password of the custom trust store. This field can be left blank if the default password of the custom trust store hasn't been modified. | No |
| HTTP Proxy Host | String | The hostname of the HTTP proxy to use to connect to IBM Rational Test Automation Server. For example, proxy.domain.com | No |
| HTTP Proxy Port | String | The port number of the HTTP proxy to use to connect to IBM Rational Test Automation Server. | No |
| HTTP Proxy User name | String | The username to authenticate with HTTP proxy. | No |
| HTTP Proxy Password | Password | The password to authenticate with HTTP proxy. | No |


|Back to ...||Latest Version|IBM Rational Test Automation Server (RTAS) ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[3.3](https://raw.githubusercontent.com/UrbanCode/IBM-UCD-PLUGINS/main/files/RTAS-UCD/RTAS-UCD-3.3.zip)|[Readme](README.md)|[Overview](overview.md)|[Usage](usage.md)|[Downloads](downloads.md)|

