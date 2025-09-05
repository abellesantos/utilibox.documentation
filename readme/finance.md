---
description: Financial efficiency
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

# Finance

Utilibox' finance module is all about making financial tasks simpler:

* Automating accounts payable tasks
* Provide spending and accrual files
* Lets you plan budgets under different scenarios
* Monitor invoice completion and validation

Also has a feature for uploading bills. Allowing users to improve the quality of their invoice data without depending on others. Its automated invoice processing offers a single digital platform for all finance functions.

<div align="left"><figure><img src="../.gitbook/assets/Finance.png" alt=""><figcaption></figcaption></figure></div>

### Accounts Payable

This feature allows users to review/edit/generate payment files for an organisation.

> _Note: accounts payable automation is only provided to organisations where the feature is enabled from the organisation configuration._

_Summary View_

This view lists all reports and provides the ability to download payment files and invoices    &#x20;

> Automated Periodical Reports
>
> This report contains details about the standard, consolidated and catch-up invoices with the option to download individual invoices and payment files User can also lock/unlock a report, refresh the report and generale emails (with zipped invoices and payment file) for submission.

_Settings_

This feature allows admin users to edit the following setting for the report:

* Delivery Mode
  * Auto
  * Review Required
* Schedule of delivery –day of the week the report will be delivered
* Recipient – email address of recipient
* Data Setting – report is shown per invoice as the default view but can be set to be aggregated in the following views:
  * None – default per invoice
  * Company
  * Retailer
  * State
  * Commodity
  * Market Segment
  * Cost Code
  * Business Unit
  * Site Code
  * Site Reference

#### Locking Process

This process allows a mandatory review of the AP file details and ability to input notes by the analyst

1. Click the “View Details” button
2. Select invoices for submission then click “Lock” at the top right corner of the page
3. Scenario 1: If all invoices are selected, there will be a simple confirmation pop-up before locking. Scenario 2: If there are excluded invoices, there will be a different confirmation process which requires the Analyst to explicitly state the reasons for exclusion.
4. Once locked, the page will indicate that the report is locked and there will be key stats per invoice type (e.g. 10 of 15 locked for submission). There is still an option to unlock the report if needed. Any excluded invoices will have a slightly different styling and there will be warning icons in the Amount column. The warning icon can be hovered to see the reason.

> _\*Unlocking Process - this process allows to include additional invoices by a metrics analyst to a locked report by clicking on the “Unlock” button._

#### Generating Email for Submission

* Allows the metrics analyst to input some notes before generating the email.
* This process generate emails for manual submission first while still at the early stages and automatically mark the report as submitted once the email is generated.
* Can also be used if manual submission is needed in case of data issues.
* During the generation process, a zip file of invoices and a payment file will be generated and will be uploaded to azure. Once generated, a .eml file will be downloaded in the browser . The email will contain clickable buttons to download the zipped invoices and payment file.
