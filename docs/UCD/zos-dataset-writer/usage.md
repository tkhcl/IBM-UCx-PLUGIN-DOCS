
z/OS Dataset Writer - Usage
===========================

# Usage



### Usage




The z/OS Dataset Writer plug-in contains the **Write to Sequential Dataset** step to write input text to a sequential dataset. For example, a JCL SYSIN content is passed as text input. Refer to the below screenshot:


[![](picture1.png?resize=320%2C130)](https://www.urbancode.com/plugindoc/zos-dataset-writer/picture1-2/)


Second input Dataset Name can either be a Sequential dataset name as below MY.SEQ.DATASET or could be a user-defined property say ```${p:sequential.dataset.name}```. The `sequential.dataset.name` property needs to be defined with a sequential dataset name for writing the input text.


[![](zos-dataset-writer-plugin.png?resize=420%2C445)](https://www.urbancode.com/plugindoc/zos-dataset-writer/picture2/)


Select checkbox **Append** to append input text data after the existing data in a given dataset. By default, **Append** is unchecked and writes the input text newly in a given dataset.


The **Allocate Data Set** and **Delete Existing Data Set** values are set to `TRUE` by default. As the name suggests, setting input **Allocate Data Set** to `TRUE` will give you an option to decide and set the parameters of a sequential dataset to be created. If **Allocate Data Set** is `FALSE`, the plug-in step assumes that the dataset exists and writes the input text to the dataset.


Input **Delete Existing Data Set** comes into action only when **Allocate Data Set** is set to `TRUE` and deletes the existing dataset. Set to **Allocate Data Set** to `TRUE` to allocate a new dataset with passed parameters and write the input text to a sequential dataset.


The remaining inputs in the step are to set parameters like DCB and Space etc., for a sequential dataset and are applicable only if **Allocate Data Set** is `TRUE`.



|Back to ...||Latest Version|z/OS Dataset Writer ||||
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|[All Plugins](../../index.md)|[Deploy Plugins](../README.md)|[2.1132365]()|[Readme](README.md)|[Overview](overview.md)|[Steps](steps.md)|[Downloads](downloads.md)|
