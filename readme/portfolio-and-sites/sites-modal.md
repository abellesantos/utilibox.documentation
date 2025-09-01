---
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
    visible: true
---

# Sites Modal

### Invoices Modal

* Settings – this allows the user to edit the date range of the invoices to be shown in the modal instead of the default last 12 months
* Site address – as setup in the organisation tree
* Commodity – as setup in the organisation tree
* Utility Identifier – as setup in the organisation tree
* Line chart that shows the spend and consumption from the last 12 months of invoices
* Total Spend and Total Consumption cards from the last 12 months of invoices
* Table Summary with the following details:
  * Period Start – date for the start of the bill period
  * Period End – date for the end of the bill period
  * Invoice Date – date invoice was issued
  * Retailer
  * Invoice Total
  * Total Consumption
  * Status – shows the state of invoice availability
    * Received
    * Missing
    * Pending
  * Validation – shows the status of the invoice validation
    * ✔️ - completed
    * ❓- incomplete data
    * ❗ - variation limits check requires review
    * N/A – bill validation is not applicable for the invoice
    * 👤
  * Actions
    * Download Invoice
    * Reparse
    * View invoice
  * Download All Invoices – action to export all invoices available on the modal based on the set date range filter

### Contracts Modal

* Site address – as setup in the organisation tree
* Commodity – as setup in the organisation tree
* Table Summary with the following details:
  * Type
  * Subtype
  * Signed
  * Start
  * End
  * Retailer
  * Actions - View Contract Rates

### Utility Details Modal

* Site address – as setup in the organisation tree
* Commodity – as setup in the organisation tree
* Utility Identifier – as setup in the organisation tree
* Network Tariff – as setup in the organisation tree from Utility Properties
* Transmission Loss Factor – as shown/parsed from the latest invoice when available otherwise as shown from the organisation tree from Utility Properties
* Distribution Loss Factor – as shown/parsed from the latest invoice when available otherwise as shown from the organisation tree from Utility Properties
* Meter Numbers – as shown/parsed from the latest invoice when available otherwise will be blank

