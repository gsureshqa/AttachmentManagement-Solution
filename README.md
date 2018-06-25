 ## Move file attachments from Dynamics 365 to Azure Blob
Move Dynamics 365 Customer Engagement aka CRM Online attachments (Notes attachments / Email Activity Mime attachments) to Azure Blob storage using Azure Attachment Management Solution
It would be ideal to test run the these Attachment Management Solution in your pre - production environments before using in your production environment.

## Description:
As a customer, I would like to move all my existing CRM attachments stored in Notes / Emails to an Azure Blob 


## Move CRM Note Attachments to Azure Blob:
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fgsureshqa%2FLAMoveCRMAttachmentsToBlob%2Fmaster%2FLA-MoveCRMNote-AttachmentsToBlob.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/>
</a>



#### Note:
To update the start and end dates for CreatedOn for email records, go to Logic App Code view -> Line 111 -> "$filter": "attachmentcount gt 0 and createdon gt 2017-01-01T00:00:00Z and createdon lt 2018-01-01T00:00:00Z",

