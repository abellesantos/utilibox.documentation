---
description: All your data in one place
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

# Portfolio and Sites

Utilibox’s site page gives customers a simple, single-screen view of all their supply point data, whether it's for electricity, gas, or water, and regardless of the size or metering of the site.

The page also offers access to contract and meter data and even allows customers to look at their recent historical invoices. This makes managing different supply points easier and more straightforward.

<figure><img src="../../.gitbook/assets/PortfolioSites.png" alt=""><figcaption></figcaption></figure>

To navigate to the Sites page--- from the toolbar menu, click on the Sites tab with the following details:

* Company | Site – this column shows the name of the company, site and supply point identifier based on how it is setup in the organisation tree. It also includes the status of the supply point identifier when it’s expired or unknown based on the start/end date setup in the organisation tree.
* Business Unit– this column shows the unit for the site provided by the organisation that is setup in the organisation tree when applicable.
* Site Code – this column shows the code for the site provided by the organisation that is setup in the organisation tree when applicable.
* Operation Status – this column shows the status of the site based on the contract terms with retailer as of current date
  * Commencing Soon – no active contract but with future contract within 6mos from current date
  * Operational – with active contract as of current date
  * Closing Soon – contract to expire within 6 months as of current date
  * Closed – expired contract as of current date
* Retailer – this column shows the name of the retailer for the most recent invoice parsed/retailer setup in the organisation tree if no invoice is available
* Final Bill Received – this column shows the bill period end date if a final invoice is received
* Contract End – this column shows the maximum contract end date based on available retail contracts.
* Estimated Spend– this column shows the estimated spend per year based on the last 12 recent available invoices
* Estimated Usage – this column shows the estimated usage per year based on the last 12 recent available invoices
* Average Rate – this column shows the yearly average rate from the estimated spend over estimated usage per year
* Tags – this is a customer-defined label for sites
* Actions
  * Invoices – a quick [link](invoices-modal.md) to view invoices from the last 12 months for the site
  * Contracts – a quick [link](contracts-modal.md) to view available contracts for the site
  * Utility Details – a quick [link](utility-details.md) to view network details of the site
