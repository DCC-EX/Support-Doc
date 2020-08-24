## DCC-EX Release Approach

DCC-EX will release products on a periodic basis.  DCC-EX Products will use GitHub's Release and Tagging approach to Releasing, Tagging and Version Numbering our Products.  Before a product is released, each product be given a DCC-EX **Release Number**, and **Version Number** Tag.

GitHub releases are a higher level concept than a version number Tag.  **Releases** are deployable iterations of software that make the sofware available for a wide audience to download and use.  Releases typically include:
   - Reease Notes
   - A number of sofware items packaged for easy distribution and installation 
   - links to binary files if those files are needed for easy distribution and installation
  

### Release Numbring
Products will be released based on the GitHub Release and Version Number system as explained in  GitHub Semantic Versioning. A Product Release will be given a Release Number as follows:
   
   aa.bb.cc where:

   **aa** - is the major number of the product
   **bb** - is the minor number of the product
   **cc** - is the fix mumber of the product

For each GitHub Release, a product may have many Version Number Tags, based on how the product was developed and tested.  The most current version number would be the most up-to-date version of the product.   

Examples of DCC-EX Production Releases are shown below:   
   Release 1.2.2 shall be the current Release of DCC++Classic
   Release 2.1.2 shall be the current Release of DCC++EX
   Release 3.0.0 shall be the first release of DCC++EX based on our new Library Architectue

Future Release of DCC-EX Products will have their Release Number incremented as needed.


### Version Numbering
Each software and documentation component of a DCC-EX Product will have its own version number as follows:  
   aa.bb.cc-suffix-x  where:

   **aa** - is the Major Version number of the product.  Major versions numbers are Incremented when there is a major change to the product that results when funcionality and/or APIs are added in a wway that they are incompatible with prior versions of the product; or when there is a major  change to the internal architecture of the product

   **bb** - is the  Minor version of the product.  Minor numbers versions are Incremented when functionality is added to the product in a backwards compatible manner

   **cc** is the Patch or Fix version of the product.  The Patch version is incremented whenever there are one or more backwards compatible Patch Fixes the product that correct a bug in the  proudct

### Version Number Suffixes and Product Assurance Testing

DCC-EX has added a number of suffuxes to the end of the Product Version Number to facilitate the DCC-EX **Product Assurance Testing or PAT** Process.   

## Product Assurance Testing
Product Assurance Testing or PAT consists of three phases, Developer Testing, Alpha Testing and Beta Testing.  PAT phases shall add an appropriate suffix to the version number tag as follows:
   - no special tag - for Developer Testing 
   - Alpha - for Alpha Testing by internal members of the DCC-EX Team
   - Beta - for Betat Testing by testers external to the DCC-EX Team who have been asked by invitation to join the Beta Testing activities. 
   **Note:** Testing Suffixes shall have a number added to the end of the Suffix which is incremented every time a new version of the Test Release is released adn re-tagged.  Several examples of this are shown below:  

      - v1.2.4-Alpha-1
      - V2.1.2-Beta-3


#### Developer Testing and Tagging
During development the developer may be adding, or modify features and fixing bugs to the product. During this phase there, yhere is no requirement to tag the developer releases. The developer can Tag these releases any way they like. 
 
### Alpha Testing and Tagging
Once the prouduct has successfully passed all of the developers tests, it is ready for testing by others, the product shall be tagged with the appropirate Product Version Number and an **Alpha** Testing Suffix shall be added to the end of the Version Number as follows:
   
   **aa.bb.cc-Alpha-x** 

and testing by other members of the DCC-EX Test Team will begin.

### Beta Testing and Tagging
Once Alpha Testing has been successfully completed, the product shall enter Bets testing, and key individuals outside the DCC-EX team, shall be asked by invitation, to test the product for a pre-planned period-of-time. The product will be re-tagged as follows:

   **aa.bb.cc-Beta-x** 

### Production Release
 Once the Beta Test period has been successfully completed, and there no major issues identified, the product shall be re-tagged as as Production Release without any Suffix and made available to everyone as follows:

    **aa.bb.cc** 



### DCC-EX Product Assurancee Testing Process 

DCC-EX Products will be released after they have successfully completed DCC-EX's **Product Assurance Testing Process (PAT)** to ensure that the products released work as expected.



### Development Phases

This section provides additional information for developers that describe the phases of the development processess.

##### Development Phase 

1. For any given Product Release, all code modules should be in the Master Branches of GitHub  
2. Developers making additions / modifications to the modules shall create their own Branch off the Master and make their changes and do their own unit and integration testing in their own Branches
3. Once a developer has completed their coding and testing, they should issue a Pull Request to Merge their Branch into the Master.
4. The DCC++EX Mgmt Team will approve Pull Requests in the sequence required and Merge the Pull Requests back into the Master

#### Alpha Testing Phase

1. Once all Pull Requests has been approved by the DCC-EX Mgmt Team the DCC++EX Chief Tinkerer shall tag that version of the Master Branch as version xx.xx.xx-Alpha and notify the Testers that it is ready for Acceptance Testing
2. Concurrently with the development, Testers shall create an Acceptance Test Plan for version xx.xx.xx-Alpha 
   a. The Test Plan will take the form of what Roger, Mani and Larry discussed today.
   b. A Tester will be asked to take the role of Key Tester. 
   c. The Key Tester will review and Approve the Test Plan, store it in GitHub along with the Name Acceptance Test for Product and Tag it with the same version as the Code xx.xx.xx
   d. The key Tester will assign Acceptance Testers and setup the Test Plan in Google Docs as we discussed today with different Tabs for each Tester
   e. Once the xx.xx.xx-Alpha version has been tagged The Testers will begin Testing the Alpha version of the code and noting which Tests Pass and which tests Fail  
   f. Once all Testers have completed their testing, as best they can, the Key Tester will identify all potential “Bugs” identified and submit a DCC++EX Bug Report for each bug identified into the GitHub DCC++EX Dev-Project
   
#### Beta Testing Phase
   
3. Once the Alpha Release passes all Acceptance Testing and there are no major Bug Reports, the DCC++EX Chief Tinker shall Merge all branches into the Master Branch and Tag that version as DCC++EX xx.xx.xx-Beta, add it to the DCC++EX Download Page and notify potential Beta Testers
   a. Beta Testers shall submit a DCC++EX Bug Report for each bug identified into the GitHub DCC++EX Dev-Project
   b. Beta Testing shall last a predetermined amount of time, of on average, One Month
   c. After the Beta Testing Time Period, he DCC++EX Mgmt Team will review all Bug Reports from the Beta Release
   d. If there are too many major or moderate bugs, the DCC++EX Mgmt Team will keep the product in Beta and continue Bug Fixing and Unit and Acceptance Testing
   e. The DCC++EX Mgmt Team will review all Tasks and Bug Reports in the Dev-Project Queue and decide which to fix and the priority and assign the work to the appropriate developer
   f. Once the developer “Fixes” the Bug on their branch of the Code and Unit Test the changes, they should a New Pull Request to Merge their Branch into the Master
   g. The process will go back to Step 4.
   
#### General Release
4. If there are no Bugs, or only minor bugs, the DCC++EX Mgmt Team will re-Tag the version as DCC++EX xx.xx.xx with no suffix and setup the product to be released to the general public
5. Users shall be encouraged to document any issues they find in the DCC++EX Support Requests which will be evaluated by the DCC++EX Mgmt Team

#### Next Release (Parallel Development)

1. While a version of a Product moves to general Product Release, the developers shall begin work on developing the  next version of the DCC++EX product.  
2. DEvelopers will create a new Development Branch of the product off of the Master Branch and begin adding new features and fixes to that Development Version of the product and go back to Step 1 of the Development Phase

    DCC++EX Release and Testing Approach  <<-- Is this for something or just didn't get deleted? What are the procedures for submitting but reports? It this "issues" with a gage?

DCC-EX Release Plan v1-Draft-A.md	

