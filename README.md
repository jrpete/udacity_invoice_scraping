# Scraping Invoice Files Using UiPath

This process downloads invoices from an email inbox, scrapes the invoice for the date, number, transaction details, Sub-total, GST %, and Total, then stories it into an Excel file. The invoice Sub-total, GST %, and Total data are then uploaded to a UiPath Orchestrator Queue and the Excel file is sent as an email attachment. 

###Installation

Clone the GitHub repositroy then use UiPath to run the "Main.xml" file. Remove any existing files from the 'Data' and 'Excel_Files' directories before running. 

```
git clone https://github.com/jrpete/udacity_invoice_scraping
cd Invoice_Scraping_Sequence
./Main.xml
```

###Usage

This project was run using UiPath Studio 2021.10.3 on a Windows 10 Home 64-bit 5.0.11 machine.

This project uses the following Dependencies: 

- UiPath.Excel.Activities v2.11.4
- UiPath.Mail.Activities v1.12.2
- UiPath.PDF.Activities v3.4.1
- UiPath.System.Activities v21.10.2
- UiPath.UIAutomation.Activities v21.10.3


### License

This project is licensed under the [MIT License](./LICENSE.md) @ Udacity


### Issues/Bugs

- To report an issue or bug, create a Pull Request and document the issue. 


### Contribution

- Jesse Peterson