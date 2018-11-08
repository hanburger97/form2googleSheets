# form2googleSheets

Instructions for google sheets setup:

1----------------------------
The Sheet

Navigate to drive.google.com and click on NEW > Google Sheets to create a new Sheet. Give it a name, perhaps “Form Google Sheets”. Put the following names into the first row of the first five columns:

    Timestamp  name  email phone message
    
2---------------------------
The Script

Click on Tools > Script Editor…, which should open a new window and a dialog called ‘Google Apps Script’. Click on Create script for > Custom Functions in Sheets. This will create one script called 'Code.gs’ containing functions such as SAY_HELLO.

Click on 'Untitled Project’ at the top and give this project a name: 'Form Script’.

Code in code.gs file

Click on the Save icon. Set the dropdown in the nav bar to 'setup’ and click on the right-pointing triangle to its left to run this function. It should show 'Running function setup’ and then put up a dialog 'Authorization Required’. Click on Continue. In the next dialog 'Request for permission - Formscript would like to’ click on Accept.

In the menus click on File > Manage Versions… We must save a version of the script for it to be called. In the box labeled 'Describe what has changed’ type 'Initial version’ and click on 'Save New Version’, then on 'OK’.

Back to the menus: click on Resources > Current roject’s triggers. In this dialog click on 'No triggers set up. Click here to add one now’. In the dropdowns select 'doPost’, 'From spreadsheet’, and 'On form submit’, then click on 'Save’.

Back to the menus: click on Publish > Deploy as web app… For 'Who has access to the app:’ select 'Anyone, even anonymous’. Leave 'Execute the app as:’ set to 'Me’ and Project Version to '1’. Click the 'Deploy’ button.

Replace the link in the success dialogue in url in google-sheet.js inside the ajax function
