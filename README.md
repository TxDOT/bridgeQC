# Bridge Hull QAQC WebApp

Description & Purpose

https://txdot.github.io/bridgeQC/webApp.html

## User Setup

Requirements & Instructions to Run Locally

## Developer Setup

### Requirements to Develop
| Required Software |
| ----------- |
| Visual Studio Code |
| Live Server Extension for VS Code |
| GitHub Desktop |


| Required Access/Permissions | Details | Access Level Needed |
| ----------- | ----------- | ----------- | 
| bridgeQC respository on GitHub | Repo within TxDOT's GitHub company, shared with Intern_2023 team | Editing Access |
| Bridge_Hull_QAQC Feature Layer on ArcGIS Online | AGO Feature layer under TXDOT_GIS AGO Account, shared with Bridge QC Group | Editing Access |
| BridgeQAQCv2 Application on ArcGIS Online | AGO Application under TXDOT_GIS AGO Account, shared with Bridge QC Group | Editing Access |
| BridgeQAQC_Tracking Dashboard on ArcGIS Online | AGO Dashboard under TXDOT_GIS AGO Account, shared with Bridge QC Group | Editing Access |

### Instructions to Develop Locally

1. Create Branch
    - A. Open file in GitHub online: [GitHub Link](https://github.com/TxDOT/bridgeQC)
    - B. Click on branch button, select "gh-pages" branch.

        ![Step1B](/REFERENCES/Readme_Developing/Step1B.png "Step1B")
    
    - C. Click on branch button again, type in the "find or create a branch..." box with the name of a new branch.

        ![Step1C](/REFERENCES/Readme_Developing/Step1C.png "Step1C")
    
    - D. Make sure that your branch will be created off of gh-pages.

        ![Step1D](/REFERENCES/Readme_Developing/Step1D.png "Step1D")
    
2. Open File in VS Code
    - A. Once your branch is created, click on the green code button.

        ![Step2A](/REFERENCES/Readme_Developing/Step2A.png "Step2A")

    - B. Make sure that local is selected, then click "Open with GitHub Desktop".

        ![Step2B](/REFERENCES/Readme_Developing/Step2B.png "Step2B")

    - C. Click on any pop ups that ask for confirmation to open in GitHub desktop.
    - D. If GitHub Desktop does not open automatically, you may have to manually open the GitHub Desktop app and find the branch.
        - a. Open GitHub Desktop.
        - b. Click on current reposity, select bridgeQC
        - c. Click on current branch, select gh-pages.
        - d. Click fetch origin.  
        - e. Now click on current branch again, you should see the branch you just made. Select it. 

            ![Step2D](/REFERENCES/Readme_Developing/Step2D.png "Step2D")
        
    - E. Click "Open the repository in your external editor".

        ![Step2E](/REFERENCES/Readme_Developing/Step2E.png "Step2E")
    
    - F. Once is VS Code, confirm at the bottom that it is the right branch and make sure that webApp.html is selected in the Explorer.

        ![Step2Fa](/REFERENCES/Readme_Developing/Step2Fa.png "Step2Fa")

        ![Step2Fb](/REFERENCES/Readme_Developing/Step2Fb.png "Step2Fb")

3. Run Live Server in VS Code
    - A. Click on "Go Live" to run the live server extension.

        ![Step3A](/REFERENCES/Readme_Developing/Step3A.png "Step3A")

    - B. Make sure that it serves on the correct port. You can change these settings in the Live Server Extension settings.

        ![Step3Ba](/REFERENCES/Readme_Developing/Step3Ba.png "Step3Ba")

        ![Step3Bb](/REFERENCES/Readme_Developing/Step3Bb.png "Step3Bb")

    - C. When the live server launches, you will have to login to AGO in order to view the app.

        ![Step3C](/REFERENCES/Readme_Developing/Step3C.png "Step3C")

    - D. You can now see any changes to the code reflected on this live server every time you save it.

4. Saving Edits
    - A. Click ctrl-s to save edits to your code as you go.
    - B. After doing a chunk of edits, click commit edits under the source control tab. Give a short message to describe your saved edits.

        ![Step4B](/REFERENCES/Readme_Developing/Step4B.png "Step4B")

    - C. Click sync changes.

        ![Step4C](/REFERENCES/Readme_Developing/Step4C.png "Step4C")

    - D. When done with your goal for the branch, you can stop the live server by clicking on port button.

        ![Step4Da](/REFERENCES/Readme_Developing/Step4Da.png "Step4Da")

    - E. Then go to GitHub Desktop. Make sure correct branch is still selected. Then click Preview Pull Request.

        ![Step4Db](/REFERENCES/Readme_Developing/Step4Db.png "Step4Db")

    - F. Make sure that it is merging into gh-pages before clicking Create pull request to confirm.

        ![Step4Ea](/REFERENCES/Readme_Developing/Step4Ea.png "Step4Ea")

        ![Step4Eb](/REFERENCES/Readme_Developing/Step4Eb.png "Step4Eb")

    - G. This should open up in GitHub online. Confirm settings before clicking Create pull request.

        ![Step4F](/REFERENCES/Readme_Developing/Step4F.png "Step4F")

    - H. If there are no conflicts, click Merge pull request on the page that pops up. If there are conflicts, go through them and resolve them first, and then click Merge pull request.

        ![Step4G](/REFERENCES/Readme_Developing/Step4G.png "Step4G")

    - I. When ready, confirm merge.

        ![Step4H](/REFERENCES/Readme_Developing/Step4H.png "Step4H")
    
    - J. Then, delete branch.
        
        ![Step4I](/REFERENCES/Readme_Developing/Step4I.png "Step4I")

    - K. Follow the same instructions to merge gh-pages into the main branch.

## Script Process Overview


## Further Documentation

