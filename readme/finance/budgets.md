---
description: Stay on track with budgets, actuals, and scenario planning—all in one place.
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

# Budgets

Budgeting can be challenging when actual spending isn’t tracked against plans. Utilibox’s Budgets feature solves this by allowing clients to create budgets, monitor spending throughout the year, and compare results. It also supports multiple scenarios for deeper analysis and smarter financial planning.

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
&#x20;              \- 10% for Environmental<br>

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
