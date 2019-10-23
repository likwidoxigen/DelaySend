# Delay Send

This script is obselete because gmail now includes schedule send. 

This script does one simple thing. It lets you delay sending email until a certain time or for a specific amount fo time. This is based off WebDigi's Gmail Scheduler with some fixes and reduced functionality/options so it just does one simple thing: Take a draft and send it at a later time. The methodology excels at easily re-usable triggers for instance, I have an end of day trigger set for "5:00pm" and a generic "2 hours later" trigger that both get used a lot.

## Delay Send features
- Private - All your emails are private, unlike third party subscription programs that need access to your entire Gmail account with read and write access.
- 100% free - No ads, No limits (Only standard Gmail outgoing limits apply).
- Open source
-- Original Source: [Link to source https://github.com/webdigi/GmailScheduler](https://github.com/webdigi/GmailScheduler)
-- Updated Source:  [Link to source https://github.com/likwidoxigen/DelaySend](https://github.com/likwidoxigen/DelaySend)
- The app is hosted on Google servers with Google app script. 

Further, you can help contribute and make it better. Please send us your feedback and any issues can be posted on the [Issue Tracker](https://github.com/likwidoxigen/DelaySend/issues)

## Delay Send Limitations
- You can only schedule ONE draft message per thread. (As many new messages may be scheduled as you would like.)

## Using Delay Send
Quick initial set up
- [Click to open Gmail Scheduler](https://script.google.com/macros/s/AKfycbyJdaHIpvEWBaTSjzl8P5dTQy_vKVeRlp4daYqa8XdeTzOa5Ek/exec)
- Accept permissions
- You'll get some hefty warnings that the app has not been reviewed. 
- Create labels as required. Feel free to add as many as you like. A pro tip is to use "2 hours later" then for days use "two days later" and so on. This means that 2 will show on the labels above two and so on. This will help make selecting the schedule easier.

Alternate (Developer) Setup
-Use an extension like "Google Apps Script Github Assistant" to pull the code into your own project.
-Deploy it as a webapp and use the generated link to manage/configure the software. 

Outgoing messages
- Now you are all set and go back to gmail and compose a message and add the label under timer as required.
- Do not click on the send button. Only set the label and then leave the message in drafts.



Accessing your GmailScheduler settings:
- https://script.google.com/macros/s/AKfycbyJdaHIpvEWBaTSjzl8P5dTQy_vKVeRlp4daYqa8XdeTzOa5Ek/exec

## Troubleshooting
1) Cannot connect to Gmail
- You might occasionally see an error that looks like the image below.
[![ErrorWithGmail](http://i.imgur.com/CNZAWhI.png)](http://i.imgur.com/CNZAWhI.png)
- The message above means that Gmail could not connect to Google app scripts. This weird timeout happens between google services and you can ignore these messages. Any queued messages will be sent out in the next run.
- If you'd like to you can set a gmail filter to delete these messages. You can filter on messages with subject "Summary of failures for Google Apps Script: Gmail Scheduler" sent from: 	apps-scripts-notifications@google.com

2) Uninstalling Gmail Scheduler
- It is quite easy to uninstall Gmail Scheduler at any time. 
- Simply visit the https://script.google.com/macros/s/AKfycbyJdaHIpvEWBaTSjzl8P5dTQy_vKVeRlp4daYqa8XdeTzOa5Ek/manage/uninstall
- Click on Uninstall (You can always follow the initial setup again to reinstall the scheduler)

### License
Delay Send is licensed under the [MIT license](https://github.com/likwidoxigen/DelaySend/blob/master/LICENSE.txt). Maintained by likwidoxigen.
