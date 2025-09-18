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
    visible: false
---

# Contract Types and Validation

#### Large Electricity Retail Contract

* Should have at least 1 site
* Energy and SEC rates section should be visible with available rates for both
  * Energy Rates
    * A user can only enter either TOU rates (peak, shoulder, offpeak) or Anytime rate
    * If TOU rate is entered, Anytime rates should be reset to 0
    * If Anytime rate is entered, TOU rates should be reset to 0
    * At least 1 rate should be valid
    * At least 1 rate should be defined
    * Overlapping rates under the same state are not allowed
  * For SEC Rates
    * Overlapping rates with the same SEC Types are not allowed
    * All fields are required
    * All fields should be valid

SME Electricity Retail Contract

* Should have at least 1 site
* Only Energy rates should be visible with available rates
* There are no SEC rates
  * Energy Rates
    * A user can only enter Anytime rate
    * Anytime rate should be defined
    * Anytime rate should be valid
    * Overlapping rates under the same state are not allowed

Large/SME Gas Retail Contract

* Should have at least 1 site
* Only Energy rates should be visible and available
* There are no SEC rates
  * Energy Rates
    * All fields are required
    * All fields should be valid
    * Overlapping rates under the same state are not allowed

Progressive Contract

* Should have at least 1 site
* Energy and SEC rates are not visible nor required
* Should be able to add a contract without any rates

LPG/Water Retail and Data Contract

* Should have at least 1 site
* Energy and SEC rates are not visible nor required
* Should be able to add a contract without any rates
