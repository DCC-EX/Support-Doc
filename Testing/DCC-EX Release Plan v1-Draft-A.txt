# DCC-EX Release and Testing Approach

DCC-EX plans to release our products on a periodic basis.  Before a product is released, each product Releases will follow a DCC-EX Testing process to ensure that the products we release work as expected for our users.  Each release will have a version number as described below: 

The first release of DCC++EX based on our new Library structure shall be called Release 03.xx.xx.  All additional release will have their release number incremented according Versions as follows:

### Version Numbers

DCC-EX uses  GitHub Semantic Versioning to version our products.  Each version will be given a version number as follows: 
					aa.bb.cc-suffix-x  where:

**aa** is the Major version of the product and is incremented when an incompatible API change is made to a product or there is a major change to the features of the product or there is a major internal architecture of the product

**bb** is the the Minor version of the product and is incremented when functionality is added in a backwards compatible manner

**cc** is the Patch version of the product and is incremented whenever there is one or more backwards compatible bug fixes

### Release Suffixes and Testing

**Developer Release** – are internal versionf of the productr that are worked on by the developers as they add new features and fix bugs.  This work is done on the developers own branch of the prodcut until the product successfully passes Developer Testing.  No specific tagging of these releases are required. 

**Release Testing Suffixes** shall be added to the end of the Version Number for the various stages of Testing as follows:

**Alpha Release**  - once developer  testing has been successfuly completed, the Developer Branch shall be merged back into the the Product Master Branch and shall be re-tagged as an Alpha Release and testing by the DCC-EX Test Team will begin. 

**Beta Release** – once Alpha Testing has been successfully completed, the product shall be re-taggest as a  Beta Release and key  individuals outside the DCC-EX team, shall be asked by invitation, to test the product for a pre-planned period-of-time. 

**Production Release** – once the Beta Test period has been completed, and there are no major issues identified, the product shall be re-tagged as as  Production Release without any Suffix and  made available to everyone.

Testing Suffixes shall have a number added to the end of the Suffix which is incremented every time a new version of the Test Release is released adn re-tagged.  Several examples of thsi are shown below:  

- v1.2.4-Alpha-1
- V2.1.2-Beta-3

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
   c. The Key Tester will review and Approve he Test Plan, store it in GitHub and the Name Acceptance Test for Product and Tag it with the same version as the Code xx.xx.xx
   d. The key Tester will assign Acceptance Testers and setup the Test Plan in Google Docs as we discussed today with different Tabs for each Tester
   e. Once the xx.xx.xx-Alpha version has been tagged The Testers will begin Testing the Alpha version of the code and noting which Tests Pass and which tests Fail  
   f. Once all Testers have completed their testing, as best they can, the Key Tester will identify all potential “Bugs” identified and submit a DCC++EX Bug Report for each bug identified into the GitHub DCC++EX Dev-Project
   Beta Testing
3. Once the Alpha Release passes all Acceptance Testing and there are no major Bug Reports, the DCC++EX Chief Tinker shall Merge all branches into the Master Branch and Tag that version as DCC++EX xx.xx.xx-Beta, add it to the DCC++EX Download  Page and notify potential Beta Testers
   a. Beta Testers shall testing submit a DCC++EX Bug Report for each bug identified into the GitHub DCC++EX Dev-Project
   b. Beta Testing shall last a predetermined amount of time, say One Month
   c. After the Beta Testing Time Period, he DCC++EX Mgmt Team will review all Bug Reports from the Beta Release
   d. If there are too many major or moderate bugs, the DCC++EX Mgmt Team will keep the product in Beta and continue Bug Fixing and Unit and Acceptance Testing
   e. The DCC++EX Mgmt Team will review all Tasks and Bug Reports in the Dev-Project Queue and decide which to fix and the priority and assign the work to the appropriate developer
   f. Once the developer “Fixes” the Bug on their branch of the Code and Unit Test the changes, they should a New Pull Request to Merge their Branch into the Master
   g. The process will go back to Step 4.  
   General Release
4. If there are no Bugs, or only minor bugs, the DCC++EX Mgmt Team will re-Tag the version as DCC++EX xx.xx.xx with no suffix and setup the product to be released to the general public
5. Users shall be encouraged to document any issues they find in the DCC++EX Support Requests which will be evaluated by the DCC++EX Mgmt Team

#### Next Release (Parallel Development)

1. While a version of a Product moves to general Product Release, the developers shall begin work on developing the  next version of the DCC++EX product.  
2. DEvelopers will create a new Development Branch of the product off of the Master Branch and begin adding new features and fixes sto that Development Version of the product and go back to Step 1 of the Development Phase
    DCC++EX Release and Testing Approach

DCC-EX Release Plan v1-Draft-A.md	

