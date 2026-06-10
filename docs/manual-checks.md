# Data Linkage Checks

TODO: Add short description.

## Purpose and Scope

This SOP provides detailed protocols for checking the CSV files of trays where the data processing query has identified too many or too few individuals for the Tray.

## Too Many Individuals: "QueryOver”

- Enter the directory “NEONIndividualLinkageChecks/QueryOver” to see what needs to be checked.   
  - Order the folder alphabetically by Name to group species together  
- For each csv in the folder:  
  - Open the csv file  
  - Click the “open with” drop-down at the top of the screen and select Google Sheets  
  - Use the File Name (species, year, domain, tray type, ID range) to locate the physical tray of specimens  
  - There will be a blank column next to “individualID” called “Present”, this is where you will enter your information.  
  - Carefully compare the list of individualID’s in the CSV with those in the tray.   
    - Enter a 1 into “Present” if the beetle is in the tray, enter a 0 if it is absent  
  - Once all of the rows have a 0 or a 1, do a check by enter \=SUM(\[interst cells here\]) at the bottom of the column  
    - This will likely autofill with cell values if the data has all be entered  
  - Compare the SUM value to the value in column “NumberOfBeetlesInTray”  
  - Ensure that it matches and **DELETE THE EQUATION**  
  - Close the file and move both the csv and the google sheet into the folder “Checked”  
  - Repeat for all files until the folder is empty and everything has been moved to “Checked”

## Too Few Individuals: "QueryUnder”

- Enter the directory “NEONIndividualLinkageChecks/QueryUnder” to see what needs to be checked.   
  - Order the folder alphabetically by Name to group species together  
- For each csv in the folder:  
  - Open the csv file  
  - Click the “open with” drop-down at the top of the screen and select Google Sheets  
  - Use the File Name (species, year, domain, tray type, ID range) to locate the physical tray of specimens  
  - There will be two blank columns next to “individualID” called “Present” and “Order”, this is where you will enter your information.  
  - Carefully compare the list of individualID’s in the CSV with those in the tray.   
    - Enter a 1 into “Present” if the beetle is in the tray, enter a 0 if it is absent  
    - For 1’s, enter their order in the box, as displayed below.
    ![Image of beetles pinned in a tray with numbers at the top left of the beetle to indicate numeric ordering. The top left beetle is labeled a 1, the beetle immediately to its right is 2, and so on, with the final beetle in the first row labeled 5 and the first beetle in the second row labeled as 6, the pattern continues with the final beetle in the last (4th) row labeled as 20. They are approximately evenly spaced, 5 per row.](assets/reference-photos/Order.png)  
  - When you find a beetle with an individualID that is not in the spreadsheet, insert a row and carefully transcribe the full individualID number from the beetle, enter a 1 in present, and record its order in the box.  
  - Once all of the rows have a 0 or a 1, do a check by enter `=SUM([interst cells here])` at the bottom of the column  
    - This will likely autofill with cell values if the data has all be entered  
  - Compare the SUM value to the value in column “NumberOfBeetlesInTray”  
  - Ensure that it matches and **DELETE THE EQUATION**  
  - Close the file and move both the csv and the google sheet into the folder “Checked”  
  - Repeat for all files until the folder is empty and everything has been moved to “Checked”

## Other things that can happen:

- Sometimes the query is incorrect because the number of beetles in the tray was counted or recorded incorrectly. If you find that the number in “NumberOfBeetlesInTray” is incorrect, update it the column
