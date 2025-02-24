# cs50_finalproject
Final project submitted for Harvard's CS50 course. Data search automation with Selenium and Google Sheets update via Google Colab.

## Problem:
In my current job, we use Google Sheets to track processes that take place within an internal system. These processes have unique numbers and are moved across different departments within the company, passing through multiple people. Through this system, we can check where the process is, when its last movement occurred, and its current status.

Since we monitor several processes simultaneously, we use a spreadsheet to record the numbers of all ongoing processes, along with their last known location, movement date, and status. This helps identify processes that may have been stuck in a certain department for too long, allowing for quick follow-ups with the responsible sector.

However, updating this spreadsheet required manually copying the process number from the sheet, pasting it into the internal system’s search tool, retrieving the updated information on date, location, and status, and then pasting it back into the spreadsheet. This had to be done one by one, consuming a significant amount of time for the person responsible for this task.

## Solution:
To address this, I created an automation script using Google Colab. This script accesses both the spreadsheet and the system’s website, automatically copying and pasting the process numbers and updating the spreadsheet with the latest date, location, and status information. This automation reduced the time required to update the spreadsheet by 90%.

## Security:
The script utilizes the authentication system of the user logged into their Google account in the browser, ensuring that no personal information is exposed. Additionally, the spreadsheet name must be explicitly specified in the code to be accessed. Another important detail is that the system's access is performed through a public search page, meaning no login credentials are required.

## Final Considerations:
This code can be adapted, with the necessary modifications, to update any Google Sheet based on data retrieved from a website. These modifications include specifying the spreadsheet name, selecting the correct website elements (via Selenium), and properly referencing the spreadsheet cells to be updated.

* The element names, rows, and columns used in the code reflect real use cases. Only the actual spreadsheet name and the system website URL have been omitted.
* The comments within the code are written in Portuguese (BR).
