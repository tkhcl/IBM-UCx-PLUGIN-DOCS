
Liquibase
=========

Liquibase is an open source tool that brings source control for tracking, managing and applying database schema changes.

This plug-in is developed and supported by the UrbanCode Deploy Community on IBM-UrbanCode’s GitHub organization. Click the “Visit Project” button at the top of the page to navigate to the project for source code, the plug-in distributable, and further information.

Downloads:
----------

* [Liquibase plug-in distribution](https://github.com/UrbanCode/Liquibase-UCD/releases)
* [Source project](https://github.com/UrbanCode/Liquibase-UCD)

If you encounter issues with the plug-in, or want to send feedback:

* See the [plug-in documentation](https://github.com/UrbanCode/Liquibase-UCD/tree/master/doc).
* Ask Liquibase plug-in specific questions on the [GitHub Issues](https://github.com/UrbanCode/Liquibase-UCD/issues) page.
* For general plug-in issues, submit questions to the [dW Answers page](https://developer.ibm.com/answers/smart-spaces/23/urbancode.html). Use the following tags: urbancode | ucdev | plugins


Available Steps
---------------

**Update**: Applies given count of change sets is specified. Else updates database to current version. **Rollback**: Rolls back change sets. **dbDoc**: Execute Liquibase in dbDoc mode to produce or update database reference documentation. **DropAll**: Drops all database objects owned by the user. **Tag**: Tags the current database state for future rollback. **Generate Changelog**: Generates change log of the database. **Export Data**: Export the data from the targeted database. **Changelog Sync**: Mark all changes as executed in the database. **Update Testing Rollback**: Updates the database, then rolls back changes before updating again. **Validate**: Checks the changelog for errors.



|Back to ...||Latest Version|
| :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[0]()|
