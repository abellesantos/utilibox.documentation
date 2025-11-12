---
description: Check invoice status and manage gaps with ease.
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
  metadata:
    visible: false
---

# Invoice Completion

Use this feature to view all supply points and check the invoice status for each billing period. If invoices are missing, you’ll find tools and actions here to help you manage and resolve them efficiently.\
\
To access this page, go to the _Finance_ menu and click on the _Missing Invoices_ tab.

_Invoice Completeness_

* this shows percentage of invoice completion based on default filters broken down by # of days it was received/processed showing invoice count.

_Main table details:_

* **Identifier** - NMI/MIRN or unique value that identifies the supply point
* **SLA** – (Service Level Agreement) indicates if a supply point has metrics service
* **LOA** – (Letter of Authorisation) indicates if a supply point has an active LOA
* **Organisation Name**
* **Company Name**
* **Commodity**
* **Site**
* **Retailer** – can have multiple instances per Identifier based on date filter
* **Contact** – Retailer email address
* **Customer ID** – Account number as shown on invoice
* **Invoice Status** – indicates the status of an invoice for their corresponding bill period represented by individual boxes
  * _Green box_ – Received
  * _Red box_ – Missing
  * _Yellow box_ – Pending (to be received)
  * _Orange box_ – Received not parsed
  * _Gray box_ – bill period is with a different retailer

#### Generate Invoice Request Email

This feature allows for an email to be created/exported in requesting invoice copies for selected supply points and sent to their designated retailer (based on contact setup in Utilibox) covering the bill period missing.

When you click on "Generate Invoice Request Email" this will download a zipped file containing the email/s that can be used to send to retailers. If there are multiple retailers on the selected supply points, it will generate individual emails per retailer.
