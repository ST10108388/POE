# PROG7312_POE_PART_1 Manual


---

### Table of Contents

- [Description](#description)
- [How To Use](#how-to-use)
- [License](#license)
---


## Description
This is an application that seeks to improve citizen engagement and service delivery through the implementation of a comprehensive municipal services application. 
This application allows users to report issues, request services, access information about local events and announcements, and lastly receive updates on the status of their service requests.
Though this version the application the only function that works is the "Report issues and request services".

#### Technologies

- Microsoft Visual Studio 2022


[Back To The Top](#read-me-template)

---

## How To go to each window
- When the application starts up the user will be presented with four buttons that each contain writing.
- The first button is the "Report issues" button, when clicked the user will be taken to the report Issues window.
- The second button is the "Local Events and Announcements" Button when clicked the user will be displayed with an error that says that the Local events and announcemnets page is unavailable.
- The third button is the "Service Requests" Button when clicked the user will be displayed with an error that says that the Service Requests page is unavailable.
- The fourth button is the "Send Feedback" button when clicked the user will be taken to the feedback window where they are able to enter their own feedback.
  
### How to add a Report
- When the user clicks the Reprot Issues button they are taken to the report issues window
- At this window the user must select the category of the issue, then enter the name of the issue, then the Location of the issue, and lastly the description
- To add an image or document to the report the user must click the upload image button
- once the add image or document button is clicked the user will be displayed with a screen a pop up screen that allows the users to select the file they wish to upload.
- Once the user has added all of the releveant information to the report they must click the save report button.
- once the save report button has been clicked the report will be saved and displayed in the table below the description textbox.
- The user has to enter every detail before saving the report.
- If the user has not entered every detail before saving the report they will be displayed with an error that says not all details have been entered.
- If the user wishes to go back to the menu they must click the Back to menu button
- If the user wishes to dsiplay the report they must click on the Display Report Button under the save report button.

### How to Display a Report
- Once the user has clicked the display report button they will be taken to the Display Report Window.
- To display a report the user must click on the report number in the table.
- Once the report number has been clicked the user will see all the textboxes fill with data from that report they will also be shown the image or document they saved with the report.
- To go back to the main menu the user must click the Back to menu button and this will take them to the main menu.
- if the user wants to go back to the add report window the user must click the Back to report button and this will take them to the add report window.

### How to send feedback
- To send feedback the user must click the send feedback button on the main menu.
- Once clicked the user will be taken to the send feedback window.
- The user must then select the overall expereicne they received when getting the service.
- The overall experience rating is from a 1 to 5, 1 being the worst service experience and 5 being the best service experience.
- the user must then enter any suggested improvements
- the user must then enter in any comment they have.
- Once all the boxes have been filled the user must then click the Submit feedback button
- if the user has not entered in all of the details the user will then be displayed with an error saying that not all of he details have been filled in.
- if the user wants to go back to the main menu they must lcick the Back to menu button.

### How to Add a announcement or event
- Click on the Local Events and Announcement button in the main menu
- After clicking the Local Events and Announcement button you will be taken to the Display Local Events and Announcements Screen
- from this screen click on the Add event or announcement button
- After clicking this button you will be taken to the add announcemnt or event screen
- from here you must enter in all the required details
- If you miss any of the details you will be displayed with an error
- if you wish to undo the event you just added you are able to click the delete event button and this will delete your event
- once you have saved all of the event you wish to add you are able to click on the  Back to display events button and this will take you to the Display events and announcements screen

### How to display an event or announcement
- First you must select the date
- Then you are able to either enter the name of the event or announcement or select a category 
- If you type in the name of the event or announcement you will be displayed with that specific event and all of the events with a similiar category will be displayed in the Recommenedd events box
- if you select the category you will be displayed with all of the events and announcements that occured on that date
- YOu are able to click the events in the Recommended events box and you will be displayed with all of the details about the event or announcement
- to display the event or announcement YOU MUST SELECT A DATE IN THE DATE PICKER.

### How to display service requests
- To display service requests the user must click on the service requests button on the main screen
- Once the button is clicked the user will be taken to the Service request management screen where they will be displayed with four blocks
- The first block is a table that shows all of the service requests and these service requests ARE ORDERED FROM HIGHEST PRIORITY AND ALSO WITH THE HIGHEST AMOUNT OF DEPENDENCIES
- an example would be if the Service request has a priority of 1 which is the highest priority and also three dependecies it will be the first service displayed in the table
- The priorities are as follows, 1 is the highest priority and the higher the number is the lower the priority of the service is.
- In the table the user is able to view the ID of the service request to track their service request.
- the user is also able to view the status,description, estimated time that the service would take to be completed, the location of the service, the workers assigned to the service, and lastly the Date the service was requested
- If a user wants to see which services depend on each other they must click on service request in the table and they will be displayed with all of the services that are dependent on each other in the square with the heading of "Services Dependent on Each Other"
- If a service request is clicked in the table they will be shown all the details of that request in the block that has the Heading of "Selected Service Request"
- In the last block the user will be displayed with the most urgent service request. This service request has the highest priority as well as the most dependencies connected to it.
- If the user wishes to go back to the main screen they are able to click on the Back To Menu button at the bottem of the window.

[Back To The Top](#read-me-template)

---

## License

MIT License

Copyright (c) [2017] [James Q Quick]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[Back To The Top](#read-me-template)

---



[Back To The Top](#read-me-template)
