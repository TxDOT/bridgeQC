# Bridge Hull QAQC WebApp

## Description & Background

- GIS WebApp developed to provide efficient editing workflow for end user conducting bridge polygon QAQC.
    - User conducts assessment of LiDAR generated polygons representative of Texas bridges.
    - Polygon regularity check is performed utilizing various visual references.
    - Edits made in app save directly to the feature layer's attribute table, updating relevant records within the database.
- Created in support of the larger TxDOT Bridge Data Aggregation Project.
    - Overall project working towards improving usability and efficacy of TxDOT bridge layer, producing bridge geometry and standardization of attributes.

## User Setup

### Requirements

| Required Access/Permissions | Details | Access Level Needed |
| --------------------------- | ------- | ------------------- |
| ArcGIS Online Account | <ul> <li> AGO login must be specifically associated to TxDOT. </li> <li> Must be an authorized member/contributor of "Bridge QC Project" AGO group. </li> </ul> | Authorized member/contributer |

<img title = "AGOGroup" src = "REFERENCES\Readme_Developing\AGOgroup.png" width = "500">

### Setup

1. Open app in browser: [Bridge Hull QAQC WebApp Link](https://txdot.github.io/bridgeQC/webApp.html)

2. Log in using TxDOT AGO credentials.

    <img title = "AGOLogin" src = "REFERENCES\Readme_Developing\AGOlogin.png" width = "300">

3. Web App should appear as below.

    <img title = "HomePage" src = "REFERENCES\Readme_Developing\HomePage.png" width = "1000">

### User Instructions and Buttonology

- [Bridge QAQC User Guide](https://txdot.github.io/bridgeQC/REFERENCES/BridgeApp_HelpDoc.pdf)


## Developer Setup

### Requirements

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

### Setup

1. Create Branch
    - A. Open file in GitHub online: [GitHub Link](https://github.com/TxDOT/bridgeQC)
    - B. Click on the branch button, select "gh-pages" branch.

        <img title = "Step 1B" src = "REFERENCES\Readme_Developing\Step1B.png" width = "350">
    
    - C. Click on the branch button again, and type in the "find or create a branch..." box. Type a name for your new branch.

        <img title = "Step 1C" src = "REFERENCES\Readme_Developing\Step1C.png" width = "350">
    
    - D. Make sure that your branch will be created off of "gh-pages".

        <img title = "Step 1D" src = "REFERENCES\Readme_Developing\Step1D.png" width = "350">
    
2. Open File in VS Code
    - A. Once your branch is created, click on the green "Code" button.

        <img title = "Step 2A" src = "REFERENCES\Readme_Developing\Step2A.png" width = "180">

    - B. Make sure that you are on the "Local" tab, then click "Open with GitHub Desktop".

        <img title = "Step 2B" src = "REFERENCES\Readme_Developing\Step2B.png" width = "400">

    - C. Click on any pop-ups that ask for confirmation to open in GitHub desktop.
    - D. If GitHub Desktop does not open automatically, you may have to manually open the GitHub Desktop app and find the branch.
        - a. Open GitHub Desktop.
        - b. Click on "Current repository", select "bridgeQC".
        - c. Click on "Current branch", select "gh-pages".
        - d. Click "Fetch origin".  
        - e. Now, click on "Current branch" again, you should see the branch you just made. Select it. 

            <img title = "Step 2D" src = "REFERENCES\Readme_Developing\Step2D.png" width = "800">
        
    - E. Click "Open in Visual Studio Code" under the "Open the repository in your external editor" option.

        <img title = "Step 2E" src = "REFERENCES\Readme_Developing\Step2E.png" width = "800">
    
    - F. Once in VS Code, confirm at the bottom that it is the correct branch and make sure that "webApp.html" is selected in the Explorer tab.

        <img title = "Step 2Fa" src = "REFERENCES\Readme_Developing\Step2Fa.png" width = "250">

        <img title = "Step 2Fb" src = "REFERENCES\Readme_Developing\Step2Fb.png" width = "250">

3. Run Live Server extension in VS Code. Live Server allows you to preview and test the WebApp as you make changes to the code.
    - A. Click on the "Go Live" button in the bottom right corner of VS Code to run the live server extension.

        <img title = "Step 3A" src = "REFERENCES\Readme_Developing\Step3A.png" width = "200">

    - B. Make sure that it is hosted on "127.0.0.1" and that it serves on the correct port (5500). You can change these settings in the Live Server Extension settings. This ensures that the redirect URI used for OAuth in the application works.

        <img title = "Step 3Ba" src = "REFERENCES\Readme_Developing\Step3Ba.png" width = "500">

        <img title = "Step 3Bb" src = "REFERENCES\Readme_Developing\Step3Bb.png" width = "400">

    - C. When the live server launches, you will have to login to ArcgIS Online in order to view the app.

        <img title = "Step 3C" src = "REFERENCES\Readme_Developing\Step3C.png" width = "300">

    - D. After you make changes and save them, the web page refreshes and reflects these edits.

4. Saving Edits to Your Code
    - A. On your keyboard, click "ctrl-s" to save edits to your code as you go.
    - B. After doing a chunk of edits, click "Commit" under the Source Control tab. Type a short message to describe your saved edits.

        <img title = "Step 4B" src = "REFERENCES\Readme_Developing\Step4B.png" width = "250">

    - C. Next, click "Sync Changes".

        <img title = "Step 4C" src = "REFERENCES\Readme_Developing\Step4C.png" width = "250">

    - D. When done with all of your edits for the branch, you can stop the live server by clicking on the "Port" button in the bottom right corner of VS Code.

        <img title = "Step 4Da" src = "REFERENCES\Readme_Developing\Step4Da.png" width = "100">

    - E. Then, go to GitHub Desktop. Make sure correct branch is still selected. Then click "Preview Pull Request".

        <img title = "Step 4Db" src = "REFERENCES\Readme_Developing\Step4Db.png" width = "800">

    - F. On the screen that pops up, make sure that it is merging into "gh-pages" before clicking "Create pull request".

        <img title = "Step 4Ea" src = "REFERENCES\Readme_Developing\Step4Ea.png" width = "400">

        <img title = "Step 4Eb" src = "REFERENCES\Readme_Developing\Step4Eb.png" width = "400">

    - G. This should open up the repository in GitHub online. Confirm settings before clicking "Create pull request".

        <img title = "Step 4F" src = "REFERENCES\Readme_Developing\Step4F.png" width = "1000">

    - H. If there are no conflicts between branches, click "Merge pull request" on the page that pops up. If there are conflicts, go through them and resolve them first, and then click "Merge pull request".

        !<img title = "Step 4G" src = "REFERENCES\Readme_Developing\Step4G.png" width = "1000">

    - I. When ready, click "Confirm merge".

        <img title = "Step 4H" src = "REFERENCES\Readme_Developing\Step4H.png" width = "1000">
    
    - J. Once the merge is successful, click "Delete branch".
        
        <img title = "Step 4I" src = "REFERENCES\Readme_Developing\Step4I.png" width = "1000">

    - K. Finally, follow the same instructions to merge "gh-pages" into the "main" branch.

## Script Process Overview

| User Action | Background Script Process |
| ----------- | ------------------------- |
| Clicks on WebApp URL and gets OAuth prompt | <ul><li>Checks if the user is already signed in.</li><li>If not signed in, asks user to sign into AGO account to verify layer permissions. </li><li>Saves token to use when/if applying edits to layer. </li><li>Loads map completely if permissions are correct. </li></ul> |
| Loads Web App | Creates map and map view: <ul><li>Creates base layers and base layer toggle.</li><li>Creates feature layers and associated renderers. </li><li>Adds all layers to map and map view. </li><li>Creates checkboxes that allow user to toggle layers on and off. </li></ul> Finds next bridge to QC: <ul><li>Queries Bridge_Hull_QAQC feature layer for those that still have Null values for the IS_IRREG field.</li> <li>Picks one bridge from the query result at random.</li> <li>Zooms to this bridge.</li> <li>Puts constraint on user's ability to zoom out or pan away from selected bridge.</li> <li>Highlights this bridge.</li> <li>Saves the Object ID of the bridge in a global variable, for later use.</li></ul> Creates Calcite Select drop-down and Comment Box for Bridge QAQC Options: <ul><li>Select has 12 options, including "Select Your Choice" which is the default selection, and does not represent an actual QAQC option.</li> <li>Comment box remains inactive until user selects an option within the irregular bridge option group.</li></ul> Creates additional buttons and widgets.|
| Clicks Skip Bridge Button | Finds next bridge to QC: <ul><li>Queries Bridge_Hull_QAQC feature layer for those that still have Null values for the IS_IRREG field.</li> <li>Picks one bridge from the query result at random.</li> <li>Zooms to this bridge.</li> <li>Puts constraint on user's ability to zoom out or pan away from selected bridge.</li> <li>Highlights this bridge.</li> <li>Saves the Object ID of the bridge in a global variable, for later use.</li></ul> Clears exisiting inputs: <ul><li> Clears any selection in the Calcite Select drop-down, and returns to default "Select Your Choice". </li> <li> Clears any inputs in Comment Box. </li></ul>|
| Selects an optin in the Calcite Select drop-down | <ul><li> Enables comment box inputs.</li> <li>Enables user to click the Save and Next Bridge button.</li></ul>|
| Clicks Save and Next Bridge Button | If user has not selected a QC option ("Select Your Choice" is still the selected option): <ul><li> An alert pops up to tell the user that there is nothing to save. </li></ul> If user has selected a QC option: <ul><li> Creates new variable to open new XML Http Request. </li> <li>Creates serviceURL variable that has basic REST URL to update features in Bridge_Hull_QAQC layer. </li> <li>Creates variables to save all of user's inputs (QC choice and comment) and append these to the service URL.</li> <li>Post edits to layer.</li></ul> Once edits get posted, finds next bridge to QC: <ul><li>Queries Bridge_Hull_QAQC feature layer for those that still have Null values for the IS_IRREG field.</li> <li>Picks one bridge from the query result at random.</li> <li>Zooms to this bridge.</li> <li>Puts constraint on user's ability to zoom out or pan away from selected bridge.</li> <li>Highlights this bridge.</li> <li>Saves the Object ID of the bridge in a global variable, for later use.</li></ul> Clears exisiting inputs: <ul><li> Clears any selection in the Calcite Select drop-down, and returns to default "Select Your Choice". </li> <li> Clears any inputs in Comment Box. </li></ul>|



## Further Documentation

#### ESRI ArcGIS Maps SDK for JavaScript Documentation

- [API reference](https://developers.arcgis.com/javascript/latest/api-reference/)

#### Reference Layer Locations

| Layer| Type | Source URL |
| ----------- | ----------- | ----------- | 
| Bridge Hull QAQC Layer | AGO Feature Service | https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/Bridge_Hull_QAQC/FeatureServer |
| Bridge Points | AGO Feature Service | https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/TxDOT_Bridges/FeatureServer  |
| Texas Roadways | AGO Feature Service | https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/TxDOT_Roadways/FeatureServer |
| Waterways | AGO Feature Service | https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/Texas_Streams/FeatureServer |
| Texas Railroads | AGO Feature Service | https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/Texas_Railroads/FeatureServer |
| Texas Imagery Service 6in Imagery | WMTS Service | https://txgi.tnris.org/login/path/food-paul-zebra-shirt/wmts/1.0.0/WMTSCapabilities.xml |
| TxDOT Vector Tile Basemap | Vector Tile Service | https://tiles.arcgis.com/tiles/KTcxiTD9dsQw4r7Z/arcgis/rest/services/TxDOT_Vector_Tile_Basemap/VectorTileServer/resources/styles/root.json |
