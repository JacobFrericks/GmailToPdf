# GmailToPdf
Gmail to PDF Google Apps Script

One of my recent projects was to create a digital filing cabinet. We got a scanner and started scanning all of our documents to put on an external hard drive, and created some Hazel scripts to automatically scan the documents for key words and place them in different folders in the digital cabinet. One thing I had to overcome, though, was those pesky email receipts. How could I automate the process to save them, and then put them in the correct folder? Well, one step was already done through Hazel, so I just had to automate getting them on my computer. My solution was to create a Google Apps script that saved the emails in a certain label as a PDF into a Google Drive folder (This can be automated with Label filters, or done manually). That folder would be saved to a Google Drive folder via the Google Drive application, and Hazel would pick it up from there and do it's automated processing/placement. 

Things learned:
Transferring information from one Google product to another Google product is a lot easier. My first attempt was to use Dropbox, but I was able to simplify the code a great deal by simply using Google Drive.

Use a temporary label. This also simplifies the code. The script will scan everything in the temporary label, process it and move it to a more permanent label. Next time it runs, it won't need to do any rescanning. This also saves processing power, especially for those with a lot of emails.
