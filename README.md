Schedule Pointe to Google Calendar
==================================

A Google Apps Script that searches Gmail's Inbox for emails sent by Schedule Pointe Inc. and creates events on Google Calendar.

## Usage

  * Adding this script to your Google Drive:
    * Open Google Apps Script editor (http://script.google.com)
    * Close the dialogue
    * Clear the myFunction() default empty function and paste the contents of [getschedule.gapps](https://raw.githubusercontent.com/igorpeixoto/Schedule-Pointe-to-Google-Calendar/master/getschedule.gapps) into the code editor
    * IMPORTANT!!!  Change the timezone to your own (it's on line 7 - const timeZone = "GMT-3";)  IMPORTANT !!!
    * File -> Save
    
  * Running the script:
    - Resources -> Current project's triggers
    - Select the following options: getSchedule, Time-driven, Hour Timer, Every Hour
    - Click on the link "notifications" (it's under the trigger otpions)
    - Select a notification to be delivered to your email in case something goes wrong with the script,
      set it to be sent while you are still awake, so you won't miss any flight.
    - When there are no new messages you will receive a notification to tell you that, this way you will know
      the script is running correctly.
    - You'll need to run the script manually one time. That's because the first time it runs it will require you to               authorize it.
    - Select Run -> getSchedule
    - Authorize it, and run it again just to make sure.

## Additional Information
  
The script will create a new spreadsheet called "Schedule Pointe to Google Calendar" in your Google Drive. It will be used to keep the script from creating duplicate events. You can also use it to keep track of the messages it processed.
  
If somehow the spreadsheet gets deleted, don't worry, the next time the script runs it will create it again.
The only problem is that you may end up having some duplicated events on your calendar (but just in the first run).

## CONTRIBUTORS

* Igor Peixoto - [Github](//github.com/mangini)

## LICENSE

Use this script at your will, for any purpose, commercial or not. 

If you want to modify and redistribute the script, just keep a reference to this repo.
