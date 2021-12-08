# **Standardizing-image-quality-control-with-fslview**

## **Description of the problem**

***fsl program*** is a very effective and useful program that is widely used in structural neuroimaging. From the processing of raw data to its analysis and combining with other data, each step is regulated by codes and is standard.However, controlling the image quality is different from other steps. A detailed control requires examining individual images manually with the ***fslview package*** (which is a subpackage of the fsl program). This means a serious waste of time and the process differs from person to person. Even in the analysis of large sample data, this process can be skipped. This can affect statistical results and standard deviations. 

## **Solution proposal**

- First of all, the image control subpackage is added under the fslview package.
- In this package, each error that disrupts the image quality is defined with a code (artefact, density difference, missing drawing of brain structures etc.)
- For this identification, _**normal limits**_ should be described for each error.
- These errors should be identified both collectively and individually (since data owners may not need to exclude some or want to check them individually).
- This package should be updated with new needs, errors and corrections. 

## **Futura direction**

Other common and important imaging programs such as ***freesurfer*** should solve this problem with similar application 
