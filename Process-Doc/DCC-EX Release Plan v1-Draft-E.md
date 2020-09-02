| DCC-EX        | Release, Version Numbering & Testing Guide |
| :------------ | :----------------------------------------: |
| **2-Sept-20** |               **V1-Draft-D**               |

## Overview



DCC-EX will periodially release its products to its customrers.  **Releases** are deployable iterations of software that make the sofware available for a wide audience to download and use.  There may be one or more prodcts in each Release. Each DCC-EX product be given a **DCC-EX Version Number** before it is released.  

### Version Numbering

The DCC-EX Project will use a variation of GitHub's **[Semantic Versioning](https://semver.org)** approach to manage version numbers for its software products and documentation as follows:

**aa.bb.cc-sufix-xx**

**Where:**

**aa** - is the Major version number of the product.  The Major Version Number starts with 1 and is incremented by 1 whenever the product funcionality  is signifacently changed; APIs are changed in a way that is incompatible with prior versions of the product; or when there is a major change to the internal architecture of the product. 

**bb** - is the  Minor version of the product.  Minor numbers versions start with O are Incremented by 1 when functionality is added to the product in a backwards compatible manner

**cc** is the Patch or Fix version of the product.  This version starts with 0 and incremented by 1 whenever there are  backwards compatible Fixe(s) to the product that correct bug(s) in the  product

**Suffix** - is the Testing Phase of the Product

**= Alpha** - indicates that the product is in Alpha Testing and it is being tested by members of the DCC-EX Team

**= Beta** - indicates that the product is in Beta Testing by testers external to the DCC-EX Team

**xx** - is a number after the suffix that indicates that the number of times the product has entered this test phase 

**Note:** **Testing Suffix Numbers** shall start with the number 1 added to the end of the **Suffix**.  This number will be incremented whenever that particular test phase must be rerun with an improved version of the software.  

- **Examples** of this are shown below:  

- **v1.2.4-Alpha-1**

- **V2.1.2-Beta-3**

  

## Software Product Test Phases

In order to insure the best possilbe product for our customers, DCC-DX uses a **Product Assurance Testing  (PAT)** process consists of three phases, **Developer **T**esting**,  **Alpha Testing** and **Beta Testing** . In many cases a product may undergo a number of internal  testing releases before it is released to customers.  In this case, a  product may have a number of different Testing  Version Number Tags depending on how the product was tested.  

 Once the Beta Test period has been successfully completed and there no major issues identified, the product shall be re-tagged as as Production Release without any Suffix and made available to everyone.  

### Developer Unit Testing

During development the developer will be adding, or modify features and fixing bugs in the product. During this phase there is no requirement to Tag the developer releases. The developer can Tag these releases any way they like. 

**Suffix = No Tag Required** -  for Developer Testing  no suffix tag is required

### Alpha Testing

Once the prouduct has successfully passed all of the developers tests, it is ready forAlpha Testing by others members of the DCC-EX Team.  At this time, the  product shall be Tagged with the appropirate Product Version Number and an **Alpha** Testing Suffix shall be added to the end of the Version Number as follows:

   **aa.bb.cc-Alpha-x** 

### Beta Testing

Once the Product enters Beta Testing, it shall be tested by individuals outside the DCC-EX team, who shall be asked by invitation to test the product.  Beta Testing will be conducted for a pre-planned period-of-time, typically one month. Upon Entering Beta Testing,the  product will be re-tagged as follows:

​    **aa.bb.cc-Beta-x** 

## Product Releases

Each DCC-EX Release may include multiple products each having its own Version Number.  For some products the Release Number and Version Number will be the same.  For other Releaes, multiple DCC-EX Products will be combined togetherinto one Releas, (For example:  A Product and several Software Libraries).  In these cases, each product may have a different version number than the Release.  

   - **Release Notes** that describe what is in the version, new features and limitations
   - **A number of software products** packaged together for easy distribution and installation
   - **Links to binary files** that are included in the release
- **Note:** There must be at least one or more software products that will be comgined into a Release 



## DCC-EX Document Versioning

DCC-EX products may be made up of software, hardware and documentation including guides, users manuals, etc. DCC-EX Documents shall have a version number similar to the product verson number:

**aa.bb.cc-sufix-xx**

**Where:**

- **aa** - is the Major version number of the document.  The Major Version Number starts with 1 and is incremented by 1 when there is a major change to the document, or when there is a major architectural change to the internal architecture of the document

- **bb** - is the  Minor version of the document.  Minor numbers versions start with O are Incremented by 1 when functionality is added to the document in a backwards compatible manner

- **cc** is the  Fix version of the document.  This version starts with 0 and incremented by 1 whenever there are  backwards compatible Fixe(s) to the product that  correct errors in the document 

- **Suffix = Draft** -while documents are still in development, the should have a **Draft Suffix** added to the end so show that they are in a Draft State followed by a Letter indicating the current version of the document.  As multiple drafts of a document  produced, the letter should be incremented through the alphabet, from A to Z.  Once a document has been Reviewed and finalized the Suffix and letter would be removed.  

- Examples of Document Version Numbers: 

  **v1.0.0-Draft-C**  - 3rd draft of the first major version of the document

  **v1.0.2** - first major version of the document with the second patch or fix

  **v3.5.9-Draft-A**  - First draft, of the third major version and fifth minor versions and one  

## DCC-EX Process Versioning

Key DCC-EX development and support processes shall also be givena version number as follows:

**aa.bb.cc-suffix-xx**

**Where:**

- **aa** - is the Major version number of the product.  The Major Version Number starts with 1 and is incremented by 1 whenever the product funcionality  is signifacently changed; APIs are changed in a way that is incompatible with prior versions of the product; or when there is a major change to the internal architecture of the product. 

- **bb** - is the  Minor version of the product.  Minor numbers versions start with O are Incremented by 1 when functionality is added to the product in a backwards compatible manner

- **cc** is the Patch or Fix version of the product.  This version starts with 0 and incremented by 1 whenever there are  backwards compatible Fixe(s) to the product that correct bug(s) in the  product

- **Suffix** - is the Testing Phase of the Product

  **= Alpha** - indicates that the process is in Alpha Testing and it is being tested by members of the DCC-EX Team
