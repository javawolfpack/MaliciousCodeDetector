MaliciousCodeDetector
=====================

Repository to keep track of revisions to my thesis project as the google play store limits how much I can include in the what's new section. This will be for those who want to be informed as to the past and ongoing status of the project. 

Updates:
V1.6.2
Resolved issue w/ standard deviation not being standard deviation
Added sending notification functionality
Forcing reprocessing/removing existing notifications 

V1.6.1
Resolved issue w/ app crashing if location is not enabled

V1.6.0
Added notifications on any found alerts
Added user feedback on any found alerts
Added notification to notify users that notifications are enabled

V1.5.2
Hopefully fixed issue in method of processing the data that was causing app to crash.

V1.5.1
Modified UI
Removed ability to disable task collection as it doesn't have an apparent battery impact, will potentially add this back if I get feedback this isn't the case.
Added more standard deviation cutoff values for user selected notification* level.
Added EULA/Research Notice with extended information about what will be collected, how the data will be transferred/stored, and details that they can not require wifi to send data now. This will only display for new users or users who have yet to start teh application. 
Added new check box that will allow user to require or not require WiFi to be enabled/connected to send data. There were a few users who mentioned that they never enable WiFi and have unlimited data so the only way to collect their data would be to allow them to disable this requirement.
Added rudimentary locking into code, which doesn't appear to work or do anything... V1.5.2 might be getting this to work to prevent multiple threads accessing the DB file simultaneously. Will be using V1.6 to represent the version with user notifications working. 
Resolved issues w/ allowing non-wifi connections
*Note Notifications still don't work



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
