# DCC-EX Release Approach

DCC-EX will release products on a periodic basis.  DCC-EX Products will use GitHub's Release and Tagging as defined in  GitHub Semantic Versioning.  Before a product is released, each product be given a DCC-EX **Release Number**, and **Version Number** **Tag**.

**GitHub Releases** are a higher level concept than **GitHubVersion Number Tags**.  **Releases** are deployable iterations of software that make the sofware available for a wide audience to download and use, and  typically include:

   - Release Notes
   - A number of sofware items packaged for easy distribution and installation 
   - links to binary files if those files are needed for easy distribution and installation

## Release Numbering

A Product Release will be given a Release Number as follows:

   **aa.bb.cc where:**

- **aa** - is the Major Version number of the product.  Major versions numbers are Incremented when there is a major change to the product that results when funcionality and/or APIs are added in a way that they are incompatible with prior versions of the product; or when there is a major  change to the internal architecture of the product
-  **bb** - is the  Minor version of the product.  Minor numbers versions are Incremented when functionality is added to the product in a backwards compatible manner
-  **cc** is the Patch or Fix version of the product.  The Patch version is incremented whenever there are one or more backwards compatible Patch Fixes the product that correct a bug in the  proudct  

 For each GitHub Release, a product may have many Version Number Tags, based on how the product was developed and tested.  

The most current version number would be the most up-to-date version of the product.   Examples of DCC-EX Production Releases are shown below:   
   Release 1.2.2 is the current Release of DCC++Classic
   Release 2.1.2 is the current Release of DCC++EX
   Release 3.0.0 is the first release of DCC++EX based on our new Library Architectue

Future Release of DCC-EX Products will have their Release Number incremented as needed.

## Version Numbering and Version Numbering Suffixes

Each software and documentation component of a DCC-EX Product will have its own version number as follows:  
   **aa.bb.cc-suffix-x**  where:

   **aa** - is the major number of the product (see above)
   **bb** - is the minor number of the product (see above)
   **cc** - is the fix mumber of the product (see above)

​	**suffix** - is the Testing Phase of the Product (see below)

​	**x** - is the number of times a new version of the product has entered this test phase 

The suffux added to the end of the Product Version Number facilitates the DCC-EX **Product Assurance Testing or PAT** Process.  The **PAT** process consists of three phases, **Developer **T**esting**,  **Alpha Testing** and **Beta Testing** and each Phase shall add an  appropriate **Suffix** to the version number tag as follows:

   - **Suffix = No Tag Required**-  for Developer Testing  

   - **Suffix = Alpha** - for Alpha Testing by internal members of the DCC-EX Team -

   - **Suffix = Beta** - for Betat Testing by testers external to the DCC-EX Team who have been asked by invitation to join the Beta Testing activities. 

      **Note:** Testing Suffixes shall have  number, **x**,  added to the end of the **Suffix** if there are a large number of errors in the Test Phase and DCC-EX Management Team decides the Test Phase must be rerun rerun with a new version of the software.  If this occurs, the **Suffix-x** is incremented every time a new version of a Test Release is released and re-tagged.  Several examples of this are shown below:  

      - **v1.2.4-Alpha-1**
      - **V2.1.2-Beta-3**

### Developer Testing and Tagging

During development the developer may be adding, or modify features and fixing bugs in the product. During this phase there is no requirement to Tag the developer releases. The developer can Tag these releases any way they like. 

### Alpha Testing and Tagging

Once the prouduct has successfully passed all of the developers tests, it is ready forAlpha Teting by by others members of the DCC-EX Team.  At this time, the  product shall be Tagged with the appropirate Product Version Number and an **Alpha** Testing Suffix shall be added to the end of the Version Number as follows:

   **aa.bb.cc-Alpha-x** 

### Beta Testing and Tagging

Once the Product enters Beta Testing, it shall be tested by  key individuals outside the DCC-EX team, who shall be asked by invitation to test the product.  Beta Testing will be conducted for a pre-planned period-of-time, typically one month. Upon Entering Beta Testing,the  product will be re-tagged as follows:

   **aa.bb.cc-Beta-x** 

### Production Release

 Once the Beta Test period has been successfully completed and there no major issues identified, the product shall be re-tagged as as Production Release without any Suffix and made available to everyone as follows:

**aa.bb.cc**

