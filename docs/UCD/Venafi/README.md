
Venafi
======


The Venafi Trust Protection Platform provides continuous monitoring and control over keys and certificates across different devices. The Venafi plug-in for IBM UrbanCode Deploy contains various steps to control Venafi certificates.


The Venafi plug-in is a community plug-in. Community plug-ins are open source projects that are developed and supported by the IBM UrbanCode development community. Click **Visit Project** at the top of the page to go to the project for further information.


Downloads:
----------

* [Source project](https://github.com/UrbanCode/Venafi-UCD)

If you encounter issues with the plug-in, or want to send feedback:

* See the [Venafi plug-in documentation](https://github.com/UrbanCode/Venafi-UCD/blob/master/Doc/UrbanCodeVenafiPlugin.pdf).
* Ask Venafi plug-in specific questions on the [GitHub Issues](https://github.com/UrbanCode/Venafi-UCD/issues) page.
* For general plug-in issues, submit questions to the [dW Answers page](https://developer.ibm.com/answers/smart-spaces/23/urbancode.html). Use the following tags: urbancode | ucdev | plugins


Available Steps
---------------

Authentication testTest the communication with the Venafi server.

Generate certificate CSRCreate a certificate signing request that may then be submitted to Venafi.

Get Certificate StatusGet information about a certificate from Venafi.

Get Venafi PolicyRetrieve the details of the Venafi policy associated with a specific policy folder.

Renew CertificateRenew a certificate.

Request CertifcateRequest a certificate from TPP.

Request Certificate WaitRequest a certificate from TPP and poll for to get the status for issuance.

Retrieve CertificateRetrieve a certificate from TPP. Certificate already exists.

Revoke CertificateRevoke a certificate.

Submit Custom Fields to VenafiSupplement a previously submitted certificate request with custom field values.

Submit CSR to VenafiSubmit the previously created CSR to Venafi for processing.

Validate Remaining DaysValidate the remaining days of a certificate before expiry. If the certificate is valid for less than the indicated number of days then the step will fail.



|Back to ...||Latest Version|
| :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[0]()|
