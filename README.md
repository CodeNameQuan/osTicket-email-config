<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Email Configuration</h1>
This tutorial will demonstrate how to set up email configuration for osTicket.<br />






<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- osTicket Installation
- Outlook 365

<h2>Installation Steps</h2>

<p>
</p>
<p>
This tutorial, I will show you how to setup your outlook to receive osTickets. For starters, make sure you are on the admin panel for osTicket. Then go to the emails tab and click "add new email". There you will fill out the form first placing the email that you want to use, the email name you could put "osTicket Support" or whatever name you would like to choose. Nextly move onto email login information section. Use the log in information you would normally use to log into outlook. Then save your progress.
</p>
  
<img src="https://imgur.com/uXzjGn9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
</p>
<p>
Next you want to set up IMAP and SMTP so that your outlook can fetch osTicket emails. So log into your outlook and go to settings, and "view all outlook settings". From there go to sync email and scroll down until you see "IMAP and SMTP settings", you will want to use the server name and port number. 
</p>
<img src="https://imgur.com/EoEcHYF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
</p>
<p>
Now that you have IMAP and SMTP settings for outlook, you want to go back into osTicket and click on the email that you just added. once it opens, go down to sending email via SMTP and fill in the server name and port number, enable it formstatus and put yes for authentication required. Now save progress to make sure it was done correctly. Once you verified thst it was done correctly, go back into the email settings and fill in the IMAP portion. Enable, fill in the server name and port number, for mailbox protocol put IMAP + SSL, for fetch frequency and emails fetched you can put whatever you feel works best for your help desk. Lastly for the fetched emails you want to click "move to folder" so that it will send the tickets to a folder in your outlook, and you can name that folder "osTicket" or whatever you choose. Save progress to make sure everything set up perfectly.
</p>  
<img src="https://imgur.com/w9mdCkR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<br />
</p>
<p>
Okay now that we have successfully added new email, you want to next go to emails, then settings. Once in settings, enable email fetching, then save.
</p>
<img src="https://imgur.com/NlnI5RW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Now you want to test the email by sending out an outgoing email, so to do that go to emails, then diagnostic. Fill in the from with the email you just created, and send it to any email that you like. When done succesfully, you should get confirmation that it was successful!
</p>
<img src="https://imgur.com/hCeuQu0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
</p>
<p>
Okay guys, wrapping up, you can go into the email that you sent the test too and you can respond back to that email. Now log into your actual outlook email and you will see that response to the test email. But you will see thst it landed inside of the main inbox, so to fix that so that your main inbox doesnt become cluttered, you want to set rules so that all " osTicket" messages goes inside of the folder you created. To set up rules, go to settings, view all outlook settings, and click on rules. Click add a new rule. Name your rule whatever you would like, for condition set it "message body includes" and then put "osTicket" for keyword. Then go to "add an action" and set it to "move to" then send it to the folder you created. And save it. Go back to the messages and you should see that all osTicket messages are in the folder you created.
</p>
<img src="https://imgur.com/Ucd1pvU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
