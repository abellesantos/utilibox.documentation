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

### Invoices

This feature shows all available invoices received and processed in Utilibox for the organisation with the following details.

> _Default view:_\
> &#x20;_- current month invoice period_\
> &#x20;_- current month issue date_\
> \
> &#xNAN;_&#x43;licking on the “View All Historical Invoices” will remove the default filters and will show all available invoices for the organisation_

* Invoice Type – this field shows the type of invoice received
  * Standard
  * Final
  * Adjustment
  * Consolidated
* Period – invoice bill period start and end date
* Retailer
* Account number
* Invoice number
* Issue date
* Property
* Reference Codes
  * Cost Code – as set up in the organisation tree
  * Retailer Code – as set up in the organisation tree
  * Asset Code
* Payment Details
  * Balance carried – amount unpaid from previous invoice/s
  * Current Amount (including GST)
  * Total due (including GST)
  * Payment due date
  * Next meter read date when available on the invoice
* Validation Status
* Actions
  * Download Invoice
  * Download csv summary
  * View Invoice File/Information
  * Reparse

### Accruals

This feature shows substitute data for periods with missing data. This provides a complete dataset to support various Utilibox modules like budgets and SME procurement. Once actual data becomes available, the accrual data will be replaced with actual data. This page shows the following details:

> _\*Only Operational Utilities are provided with accrual data_
>
> _Default view:_
>
> &#x20;\- current month invoice period
>
> _\*Clicking on the “View All Historical Invoices” will remove the default filters and will show all available accruals for the organisation._

* Property
  * Site Name
  * Commodity – shown as a symbol
  * Utility Identifier
  * Closure date when applicable
* Reference Codes
  * Cost Code – as set up in the organisation tree
  * Retailer Code – as set up in the organisation tree
  * Asset Code
* Last Invoice Details
  * Period – date of the service period for the invoice
  * Balance carried – amount unpaid from previous invoice/s
  * Current Amount (including GST)
  * Total due (including GST)
  * Payment due date
* Accrual Details
  * Period – date of the service period for the accrual
  * Spend – estimated amount
  * Usage – estimated usage
  * Effective rate – estimated rate
  * Method references – data used to calculate for the estimate
* File Download – allows for a csv file to be downloaded for the accrual line

### Budgets

This feature allows clients to create budgets and track actual spending against the budget set throughout the year. A client can create multiple scenarios that they can analyze.

_Main Data Sources:_

* Latest successfully parsed invoice(s) – doesn’t necessarily mean the invoice from the most recent period, instead the latest invoice available in UB.
* Accruals as substitute for missing actual data from invoices
* Retail Contract Rates
* EAPI – Energy Action price index containing data from past auctions
* Environmental Certificate rates
* Environmental Compliance %
* Network Spend % change per Market Segment (C\&I/SME)
* For Bundled - % cost allocations to unbundled energy spend, network spend and environmental spend

_Estimation Methods:_

* Baseline costs: average of prior invoices
* Baseline and forward usage 1: data from same period of prior year
* Non-bundled electricity energy spend 1 (no contract in place for budget period): data from same period of prior year with applied adjustments based on retail price index movement (when there is no contract)
* Non-bundled network spend: data from same period of prior year with applied adjustments based on network price movement
* Non-bundled network electricity energy spend 2 (contract in place for budget period): estimate based on usage from same period of prior year and contract rates
* Non-bundled electricity energy spend 3 (contract in place for part of budget period only): estimate based on usage from same period of prior year and combination of contract rates and retail price index
* Non-bundled enviro spend 1 (contract in place for part of budget period only): estimate based on usage from same period of prior year and combination of contract rates and certificate price index
* Non-bundled enviro spend 2 (no contract in place for budget period): estimate based on usage from same period of prior year and certificate price index
* Non-bundled other spend: estimate based on usage from same period of prior year and rate from latest invoice
* Bundled energy spend: unbundled estimate from June in prior year data to June in previous year with applied adjustments based on retail price index movement
* Bundled network spend: unbundled estimate from prior year data with applied adjustments based on network price movement
* Bundled enviro spend: unbundled estimate from prior year data with applied adjustments based on certificate price index movement
* Bundled other spend: unbundled estimate from prior year data
* Unbundled estimate from latest invoice
* Import budget: custom calculations – this is the default for imported budget scenarios

_**BASELINE ESTIMATION**_\
&#xNAN;_&#x46;or non-bundled_\
\- actuals/accruals from prior year are used

_For bundled/SME_\
\- bundled spend from prior year and % cost allocations for Energy Spend, Network Spend and       Environmental Spend will be applied. If there are no defined % cost allocations, the followingdefaults will be applied:\
&#x20;              \- 50% for Energy\
&#x20;              \- 40% for Network\
&#x20;              \- 10% for Environmental

_**BUDGET ESTIMATION**_\
&#xNAN;_&#x45;stimated Energy Spend_\
\- for past or current period – will utilize the latest successfully parsed invoice(s)\
\- for future period and with an active contract for the utility during the budget period

* C\&I – retail spend will come from:
  * Average rate from latest invoice
  * Average rate from contract rates
  * EAPI rates for days not covered by contract
  * Utility’s estimated usage based on prior year
* Bundled/SME
  * Unbundled Energy Spend baseline
  * % change of retail price index (prior period vs budget period)

\- if estimation fails from the above and no market index is available, default to market rates or rates from the last invoice will be utilized

* Electricity C\&I – latest retail price index for the state
* Electricity SME or WA bundled – estimate based on EAPI for the state and rough estimate of 50% energy costs for bundled energy invoices
* Gas – rate from latest invoice multiplied by utility’s estimated usage based on prior year

_Estimated Network Spend_\
\- apply relative network spend changes if applicable, else use data from prior period (same approach for both Electricity, Gas, C\&I and SME)\
\- data reference can be exported in the EAX admin > Networks page

_Estimated Environmental Spend_\
\- for past or current period – will utilize the latest successfully parsed invoice(s)\
\- for future period and with an active contract for the utility during the budget period

* C\&I – environmental spend will come from:
  * Contract Supply Point average rate
  * Latest environmental certificate rate for days not covered by contract
  * Utility’s estimated usage based on prior year
* SME

\- if estimation fails from the above and no market index is available, default to market rates or rates from the last invoice will be utilized

* Electricity C\&I – latest environmental certificate rate for the state
* Electricity SME – 0

_Estimated Other Spend_\
\- sum of prior period’s Adjustments, Market Charges, Metering Charges and Other Charges
