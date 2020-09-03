| DCC-EX        | Release, Version Numbering & Testing Guide |
| :------------ | :----------------------------------------: |
| **3-Sept-20** |               **V1-Draft-E**               |

## Overview



Periodialy DCC-EX will release products to its customrers.  **Releases** are deployable software components that are made  available for a wide audience to download and use.  There may be one or more products in each Release. Each DCC-EX product shall be given a **Version Number** as it is released.  

## Software Versioning

DCC-EX will use a variation of GitHub's **[Semantic Versioning](https://semver.org)** and GitHub Releases and Tags  to manage version numbers for its software products  as follows:

**aa.bb.cc-sufix-xx**

**Where:**

**aa** - is the Major version number of the product.  Major Version Numbers starts with 1 and are incremented by 1 whenever the product funcionality  is signifacently changed; whenever APIs are changed in a way that is incompatible with prior versions of the product; or when there is a major change to the internal architecture of the product. 

**bb** - is the  Minor version of the product.  Minor numbers versions start with 0 and are Incremented by 1 when functionality is added  in a backwards compatible manner

**cc** is the Patch or Fix version of the product. Patch version numbers starts with 0 and are incremented by 1 whenever there are  backwards compatible Fixe(s) to the product that correct bug(s) or other issues in the  product

**Suffix** - is the Software Product Testing Phase that the product is in  (See next section for more details on Software testing Phases)

**Suffix = Alpha** - indicates that the product is in Alpha Testing and it is being tested by members of the DCC-EX Core Team

**Suffix = Beta** - indicates that the product is in Beta Testing by testers external to the DCC-EX Team

**xx** - is a Testing Suffix Number after the suffix.  Testing Suffix Numbers shall start with the number 1 and are incremented by 1 whenever that particular test phase must be rerun with corrections to issues found in the  the software.  

- **Examples** of this are shown below:  

- **v1.2.4-Alpha-1**

- **V2.1.2-Beta-3**

  

## Software Product Test Phases

In order to insure the best possilbe products for our customers, DCC-DX uses a **Product Assurance Testing  (PAT)** process consists of three phases, **Developer **T**esting**,  **Alpha Testing** and **Beta Testing** as shown below:

### Developer Unit Testing

During development the developer will be adding, or modifying product features and fixing bugs in the product. During this phase there is no requirement to Tag the developer releases. 

**Suffix = No Tag Required** -  for Developer Testing  no suffix tag is required

### Alpha Testing

Once the prouduct has successfully all of the developers tests, it is ready forAlpha Testing by others members of the DCC-EX Team.  DCC-EX shall develop stndard  Product Test Plans so as to  provide a cosistent means of teting each product.  If bugs are found in the product during Alpha Testing, the Alpha Testers shall fill out a DCC-EX Support Request to document the issue in a consistent way so that the  root cause be identified and a fix provided. At this time, the  product shall be Git Tagged with the appropriate Product Version Numberdependent of what was changed in the product (see product versions above) and an **Alpha** Testing Suffix shall be added to the end of the Version Number:

   **aa.bb.cc-Alpha-x** 

### Beta Testing

Once the Product has successfuly passed Alpha Testing, it will enter Beta Testing, In Beta Testing the product shall be tested by individuals outside the DCC-EX Core Team, who shall be asked by invitation to test the product. The Beta Testers  shall be given DCC-EX developed Product Test Plans to help them consistently test the product. Beta Testers shall also be able to develop and use their own tests during Beta Testing. If bugs are found during Beta Testing, the Beta Testers shall be requested to fill out a DCC-EX Support Request to document the issue in a consistent way and to notify the DCC-EX Team so that the root cause of the issue be identified and a fix provided.  Beta Testing will be conducted for a pre-planned period-of-time to be determined by DCC-EX Development and Management Team. Upon Entering Beta Testing,the  product will be re-tagged as follows:

​    **aa.bb.cc-Beta-x** 

### Production Releases

Once the product has successfully passed Beta Testing, it will be ready for general Production Release.  Each Release may include one or more  products each having its own Version Number.  For some products the Release Number and Version Number may be the same.  For other cases where, multiple DCC-EX Products are combined together into one Release, each product may have a different version number than the Release.  In addition to software, Releases shall also contain:

   - **Release Notes** that describe what is in the release in terms of new features and functions as well as any limitations
   - **One or more software products** packaged together for easy distribution and installation
   - **Links to binary files** that are included in the release

## Document Versioning

DCC-EX  also provides documentation including guides, users manuals, etc.Each  DCC-EX Documents shall have a version number similar to the product verson number as follows:

**aa.bb.cc-sufix-xx**

**Where:**

- **aa** - is the Major version number of the document.  Major Version Number shall start with 1 and are incremented by 1 when there is a major change to the document.

- **bb** - is the  Minor version of the document.  Minor numbers versions start with 0 are Incremented by 1 when functionality is added to the document in a backwards compatible manner

- **cc** is the  Fix version of the document.  This version starts with 0 and incremented by 1 whenever there are  backwards compatible Fixe(s)  that  correct errors in the document 

- **Suffix = Draft** - while documents are still in development, the shall  have a **Draft Suffix** added to the end of the document version number to  show that they are in a Draft State, followed by a Letter indicating the current version of the document.  As multiple drafts of a document are produced, the letter should be incremented through the alphabet, from A to Z.  Once a document has been Reviewed and finalized the Suffix and letter would be removed.  

- Examples of Document Version Numbers: 

  **v1.0.0-Draft-C**  - 3rd draft of the first major version of the document

  **v1.0.2** - First major version of the document with the second fix of a document

  **v3.5.2-Draft-A**  - First draft, of the third major version and fifth minor versions and second fix of the doccument  

## Process Versioning

Key DCC-EX development and support processes shall also be given a version number as follows:

**aa.bb.cc-suffix-xx**

**Where:**

- **aa** - is the Major version number of the process.  Major Version Number shall start with 1 and are incremented by 1 whenever the process funcionality  is signifacently changed 

- **bb** - is the  Minor version of the process.  Minor numbers versions start with 0 and are Incremented by 1 whenever minosr functionality is added to the process in a backward compatable manner

- **cc** is the Fix version of the process.  The Fix  version starts with 0 and is incremented by 1 whenever there are  backwards compatible Fixe(s) to the process that correct bug(s) in the  process

- **Suffix** - is the testing Phase of the process

  **Suffix  = Alpha** - indicates that the process is in Alpha Testing and it is being tested by members of the DCC-EX Team
  
  If the process affects users outside of the DDCc-EX Core Team,  the process may enter a Beta Testing phase where DCC-EX users are asked to help test the procerss. In this case, the Suffix shall be changed to:
  
  **Suffix = Beta** - indicates that the process is in Beta Testing and it is being tested by members outside of the Core DCC-EX Team