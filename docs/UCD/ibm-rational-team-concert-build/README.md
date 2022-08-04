
IBM Rational Team Concert - Build
=================================

No source configuration plug-in is required to use Rational Team Concert builds in IBM UrbanCode Deploy.

View a demo of this capability [here](https://youtu.be/1WSpLKsekr0). Read about a full deployment architecture and process using WAS, BPM, and RTC [here](https://community.ibm.com/community/user/wasdevops/blogs/laurel-dickson-bull1/2022/07/20/bpserver).

You can now continuously build and deploy your applications with Rational Team Concert Build and IBM UrbanCode Deploy. You can use IBM UrbanCode Deploy to define the application components and the processes that are required to manage an application in test and production environments. The IBM UrbanCode Deploy process design tool makes it easy to define the steps required to deploy a new version of an application.

![process_design](process_design-300x288.png)

A Rational Team Concert build creates the files that run your application, such as .jar, .war, and .ear files. The post-build deploy option makes it easy to create a new component version in IBM UrbanCode Deploy and to upload those files to that version.

![component_version](component_version-300x97.png)

Then, you can configure the post-build deploy option to have IBM UrbanCode Deploy run an application process. IBM UrbanCode Deploy runs the steps in the process to deploy them in a live environment with minimal or no down time.

![application_process](application_process-300x201.png)

When the build is complete, the application process runs, and customers can continuously use the latest features.


|Back to ...||Latest Version|
| :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[0]()|
