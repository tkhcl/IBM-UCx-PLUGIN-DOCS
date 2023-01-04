
# IBM z/TPF Beta

IBM z/Transaction Processing Facility is a high-performance and high-reliability transaction processing operating system for airline, rail, and hotel reservations, and financial transactions systems.

The z/TPF Deploy beta plug-in runs a ZOLDR LOAD command and then a ZOLDR ACTIVATE command on the target z/TPF system. The z/TPF Undeploy beta plug-in runs a ZOLDR DEACTIVATE command and then a ZOLDR DELETE command on the target z/TPF system. The z/TPF Commit beta plug-in runs a ZOLDR ACCEPT command on the target z/TPF system. Together these three plug-ins for IBM UrbanCode™ Deploy can automate the build, promotion, and deployment of artifacts to z/TPF test and production systems, as part of a continuous delivery environment.

### Disclaimer

These plug-ins are in beta. The interface, functions, and processes of the plug-ins might change. This information is for planning purposes only. The information herein is subject to change or removal without notice before the products described may become available.

### Compatibility and Platform Support

The z/TPF plug-ins have the following requirements to run on your z/TPF system:

* APAR [PJ43978](http://www-01.ibm.com/support/docview.wss?uid=swg1PJ43978) is applied to your z/TPF system.
* At least one LNIATA interface is configured and assigned for communication between the IBM UrbanCode Deploy agents and the z/TPF system.
* The z/TPF system is in the NORM state.
* The debug server must be started on the z/TPF system. To start the debug server, enter ZINET START S-DBUG.
* The access control rule is enabled for IBM UrbanCode Deploy to access the z/TPF system. To enable this rule, enter the ZDBUG ACCESS command with the ALTER and URBAN parameters specified.

The z/TPF plug-ins require IBM UrbanCode™ Deploy 6.1 or later.

### Installation

See [Installing plug-ins in IBM UrbanCode products](https://community.ibm.com/community/user/wasdevops/blogs/laurel-dickson-bull1/2022/06/13/install-plugins).

### Release Notes

See the Starter Kit Guide of [IBM UrbanCode Deploy plug-ins for IBM z/TPF](http://www-01.ibm.com/support/docview.wss?uid=swg24042652) for environment setup and configurations.


|Back to ...||Latest Version|
| :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[0]()|
