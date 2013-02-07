MaliciousCodeDetector
=====================

Repository to keep track of revisions to my thesis project as the google play store limits how much I can include in the what's new section. This will be for those who want to be informed as to the past and ongoing status of the project. 

Updates:

V1.5.0
Added data processing back into application
Modified data processing from earlier versions to be smarter
Only processes new data
Updates database with statistics resulting from the processing results, which will be used in the notification system (next step)
Added check to stop sending/processing if phone becomes unplugged partway through

V1.4.2 
Robust sending added that will try sending again a few times if the first send fails. 

V1.4.1 
Reversed send order to prioritize sending newer data and only query the database for data that hasn't been sent to make sending more efficient. 

V1.4 
Added multi-thread send support to make better use of the CPU to do the sends, additionally for users with devices Honeycomb+ making use of high performance wifi to allow sends to happen faster. 

V1.3 
Added check that send actually occurs before I record it sent in the app, will insure data actually gets sent in the future.
