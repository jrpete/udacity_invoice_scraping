Program a Robot that will “Read the last unread emails” from your mail.

Program a Robot that will download all the attachments with a naming convention of CustomerName_InvoiceDate_InvoiceNumber.pdf file from the mail with the subject line Techno Computers.

Program a Robot to save the attachment files in the data folder which has already been created or create it in the Project directory.

Regex
[a-zA-Z]+_\d{8}_\d+.pdf

Program a Robot that will “extract the relevant fields from the document”:

InvoiceNo			pdfArray(17)
InvoiceDate			pdfArray(18)

Order Information   starts at 21
	ItemNo	
			pdfArray(counter).Split(" "c)(0)
	Description
			pdfArray(counter).Substring(3,pdfArray(counter).Length-colLength)
	Quantity
			pdfArray(counter).Split(" "c)(pdfArray(counter).Split(" "c).Length-3)
	Price
			pdfArray(counter).Split(" "c)(pdfArray(counter).Split(" "c).Length-2)	
	SubTotal
			pdfArray(pdfArray.Length-3)
	GST
			pdfArray(pdfArray.Length-2)
	Total
			pdfArray(pdfArray.Length-1)


Program a Robot to save the all Order Information details into an excel sheet and save the excel sheet as “CustomerName_InvoiceNumber.xlsx”

Program the bot to upload the following Order Information details to the Orchestrator Queue:
SubTotal
GST
Total
Program the bot to email the excel file as an attachment to yourself with the subject line as “Course 2 Automation: CustomerName_InvoiceNumber details uploaded to queue”.
Repeat Step 4-7 for the remaining invoices.
Program the robot to successfully end if all the attachments downloaded from the mail in Step 2 are processed.
Fill out the Process Definition Document based on the Process Definition Document Overview & Instructions below.
Create a recording of a walkthrough of your automation following the Video Walkthrough Guidelines listed below.