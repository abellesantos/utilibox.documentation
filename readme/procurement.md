---
description: Agile procurement
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

# Procurement

Utilibox offers tools for understanding energy market data, handling procurement, and managing contracts. Providing energy market data such as electricity futures, spot prices for electricity and gas, a business contract price index, and environmental certificate prices.

On the contract management side, Utilibox serves as a storage for contract documents, tracking contract prices, and sending alerts about contract end dates. Making it easier for businesses to keep on top of their energy markets and contracts.

<figure><img src="../.gitbook/assets/Procurement.png" alt=""><figcaption></figcaption></figure>

This page allows users to create/update procurement events, contracts and displays available data source for AU market pricing.

To navigate to the Procurement page--- from the toolbar menu click on Procurement which would show the following pages:

<figure><img src="../.gitbook/assets/Procurement Toolbar.gif" alt=""><figcaption></figcaption></figure>

### Procurement Events

This feature allows users to manage and create procurements for SME customers and present the available offers from different participants and be able to compare and choose the best offer for their needs.

_Note: Customers are not allowed to add, edit or delete procurement events_

### Contracts

This feature shows contracts available for the organisation and allows users to add, update and delete contracts.

Contract Status Tracking

* Future – contract with start date greater than 6 months from current date
* Commencing Soon – contract with start date within 6 months from current date
* Current – contract start and end date is within current date
* Expiring soon – contract with end date within 6 months from current date
* Expired – contract end date is less than current date

Supported Contract Types and Validation Specifications

* _Large Electricity Retail Contract_
  * Should have at least 1 site
  * Energy and SEC rates section should be visible with available rates for both
    * Energy Rates
      * A user can only enter either TOU rates (peak, shoulder, offpeak) or Anytime rate
      * If TOU rate is entered, Anytime rates should be reset to 0
      * If Anytime rate is entered, TOU rates should be reset to 0
      * At least 1 rate should be defined
      * At least 1 rate should be valid
      * Overlapping rates under the same state are not allowed
    * For SEC Rates
      * Overlapping rates with the same SEC Types are not allowed
      * All fields are required
      * All fields should be valid



* _SME Electricity Retail Contract_
  * Should have at least 1 site
  * Only Energy rates should be visible with available rates
  * There are no SEC rates
    * Energy Rates
      * A user can only enter Anytime rate
      * Anytime rate should be defined
      * Anytime rate should be valid
      * Overlapping rates under the same state are not allowed



* _Large/SME Gas Retail Contract_
  * Should have at least 1 site
  * Only Energy rates should be visible and available
  * There are no SEC rates
    * Energy Rates
      * All fields are required
      * All fields should be valid
      * Overlapping rates under the same state are not allowed



* _Progressive Contract_
  * Should have at least 1 site
  * Energy and SEC rates are not visible nor required
  * Should be able to add a contract without any rates



* _LPG/Water Retail and Data Contract_
  * Should have at least 1 site
  * Energy and SEC rates are not visible nor required
  * Should be able to add a contract without any rates

