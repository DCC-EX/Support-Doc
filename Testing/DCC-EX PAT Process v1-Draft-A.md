### DCC-EX Product Assurance Testing Process

DCC-EX Products will be released after they have successfully completed DCC-EX's **Product Assurance Testing Process (PAT)**. This process will ensure that DCC-EX users get the best product possible. This section provides additional information for developers that describe the phases of the development processess.

### Release Setup

Once the DCC-EX Management Team determines that a new Product Release shall begin, they will create a new GitHub Release with some preliminary information about the Release.  

### Development Phase

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

