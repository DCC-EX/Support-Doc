# DCC-EX Release & Testing Naming Conventions

DCC-EX Products will use GitHub's **[Semantic Versioning](https://semver.org)** approach to managing  version numbers for its software products and documentation.  Semantic Versioning provides a simple set of rules and requirements that determine how product version numbers are assigned and incremented. Before a product is released, each product be given a DCC-EX **Version Number** **Tag**.

## Product Releases

DCC-EX will periodially release its products to its customrers.  **Releases** are deployable iterations of software that make the sofware available for a wide audience to download and use, and  typically include:

   - Release Notes that describe what is in the version, new features and limitations
   - The sofware items each with their own version number packaged together for easy distribution and installation
   - Links to binary files that are included in the release
   - **Note-1:** There must be at least one software product and there may be multiple products that are comgined into a Release 
   - **Note-2:** Version numbering and release numbering are closely related for most software products as you will see below

### Release Numbers are provided for each product as follows:  

​			 **Major.Minor.Patch**

**Where:**

- **Major** - is the Major Release or Version number of the product.  Major versions numbers are Incremented when there is a major change to the product that results when funcionality and/or APIs are added in a way that they are incompatible with prior versions of the product; or when there is a major architectural change to the internal architecture of the product
- **Minor** - is the  Minor version of the product.  Minor numbers versions are Incremented when functionality is added to the product in a backwards compatible manner
- **Patch** is the Patch or Fix version of the product.  The Patch version is incremented whenever there are one or more backwards compatible Patch Fixes to the product that correct a bug in the  product

## Software Product Version Numbering and Test Phase

Each DCC-EX Release may include multiple products each having its own Version Number.  For some products the Release Number and Version Number will be the same.  For other Releaes, multiple DCC-EX Products will be combined togetherinto one Releas, (For example:  A Product and several Software Libraries).  In these cases, each product may have a different version number than the Release.  

In many cases a product may undergo a number of internal  testing releases before it is released to customers.  In this case, a  product may have a number of different Testing  Version Number Tags depending on how the product was tested.  

Each software  component of a DCC-EX Product will have its own version number as follows: 


   **Major.Minor.Patch-Suffix-x**  

**Where:**

   **Major** - is the major version of the product (see above)
   **Minor** - is the minor version of the product (see above)

  **Patch** - is the patch or fix version of the product (see above)

​	**Suffix** - is the Testing Phase of the Product (see below)

​	**x** - is a number after the Suffix that indicates that the number of times a version of the product has entered the test phase 

The **Suffux** is added to the end of the Product Version Number to facilitate the DCC-EX **Product Assurance Testing or PAT** Process.  The **PAT** process consists of three phases, **Developer **T**esting**,  **Alpha Testing** and **Beta Testing** and each Phase shall change the **Suffix** as follow below:

### Developer Testing and Tagging

During development the developer will be adding, or modify features and fixing bugs in the product. During this phase there is no requirement to Tag the developer releases. The developer can Tag these releases any way they like. 

**Suffix = No Tag Required**-  for Developer Testing  no suffix tag is required

### Alpha Testing and Tagging

Once the prouduct has successfully passed all of the developers tests, it is ready forAlpha Testing by others members of the DCC-EX Team.  At this time, the  product shall be Tagged with the appropirate Product Version Number and an **Alpha** Testing Suffix shall be added to the end of the Version Number as follows:

   **Major.Minor.Patch-Alpha-x** 

**Suffix = Alpha** - indicates that the product is in Alpha Testing and it is being tested by  members of the DCC-EX Team

### Beta Testing and Tagging

Once the Product enters Beta Testing, it shall be tested by individuals outside the DCC-EX team, who shall be asked by invitation to test the product.  Beta Testing will be conducted for a pre-planned period-of-time, typically one month. Upon Entering Beta Testing,the  product will be re-tagged as follows:

​    **Major.Minor.Patch-Beta-x** 

**Suffix = Beta** - indicates that the product is in Beta Testing by testers external to the DCC-EX Team

**Note:** **Testing Suffixes** shall start with the Number 1 added to the end of the **Suffix**.  This number will be incremented whenever the DCC-EX Management Team determines that that particular test phase must be rerun  with an improved version of the software.  Several examples of this are shown below:  

- **v1.2.4-Alpha-1**
- **V2.1.2-Beta-3**

### Production Release

 Once the Beta Test period has been successfully completed and there no major issues identified, the product shall be re-tagged as as Production Release without any Suffix and made available to everyone as follows:

**Major.Minor.Patch**

The most current Release  Number would be the most up-to-date version of the product.   Examples of DCC-EX Production Releases are shown below:

- **Release 1.2.2 is the current Release of DCC++Classic**

- **Release 2.1.2 is the current Release of DCC++EX**

- **Release 3.0.0 is the first release of DCC++EX based on our new Library Architectue**

  

## DCC-EX Document Versioning

DCC-EX products may be made up of software, hardware and documentation including guides, users manuals, etc. DCC-EX Documents shall have a version number similar to the product verson number:

**Major.Minor.Patch**

**Where:**

- **Major** - is the Major Version number of the doument.  Major versions numbers are Incremented when there is a major change to the document that results when funcionality it describes or the APIs described are added in a way that they are incompatible with prior versions of the product; or when there is a major architectural change to the internal architecture of the document
- **Minor** - is the  Minor version of the document.  Minor numbers versions are incremented when significant functionality is added to the product description in a backwards compatible manner
- **Patch** is the Patch or Fix version of the document.  The Patch version is incremented whenever there are one or more backwards compatible Patch Fixes  that correct errors in the document 

While documents are still in development, the should have a **Draft Suffix** added to the end so show that they are in a Draft State followed by a Letter indicating the current version of the document.  As multiple drafts of a document may be produced, the letter would increment through the alphabet, from A to Z.  Once a document has been Reviewed and finalized the Suffix and letter would be removed.  Some Examples:

**v1.0.0-Draft-C**  - 3rd draft of the first major version of the document

**v1.0.2** - first major version of the document with the second patch or fix

**v3.5.9-Draft-A**  - First draft, of the third major version and fifth minor versions and one  