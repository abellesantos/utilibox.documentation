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

# Organisation Tree

Managing multiple subsidiaries and sites can quickly become overwhelming without a clear structure. The Organisation Tree solves this by giving admin users a structured view of the entire hierarchy, making it easy to manage entities, subsidiaries, and site details within one central place.



* **Company** – business name as shown in an invoice and is usually the listed name incorporated with the ABN
* **Site** – name of the site of the company but defaults to the address of the site unless otherwise specified
  * _Company (Parent)_ – this field shows the company name the site is under and can be updated if a site needs to be moved from one company to another via a dropdown list of available companies under the organisation.
  * _Site Name_ – this field shows the name of the site that is defaulted to the site address unless otherwise specified
  * _Cost Code_ - this field shows the code for the site provided by the organisation when applicable.
  * _Business Unit_ – this field shows the unit for the site provided by the organisation when applicable.
  * _Site Code_ – this field shows the code for the site provided by the organisation when applicable.
  * _Site Reference_ – this field shows the reference name for the site provided by the organisation when applicable.
* **Address** – shows the address of the site or business as listed in an invoice and can be setup to be the physical or billing address (or both) of the site.
  * _Site (Parent)_ – this field shows the site name the address is under and can be updated if an address needs to be moved from one site to another via a dropdown list of available sites under the organisation.
  * _Search for Address_ – this field allows for an automated search of an address using Google. User would only need to enter the address, and it automatically searches for the complete and correctly formatted address.
  * _Formatted Address_ – this field shows the correct format and full address of a site based on the individual fields setup in the organisation tree.
  * _Unit Number_
  * _Street_
  * _Suburb_
  * _State_
  * _Country_
  * _Postcode_
  * _Type_ – this field has a dropdown list that shows if an address is the physical or billing address of the site
  * _Is Primary_ – if there are multiple addresses for a site, this can be enabled to determine if an address is their primary address.
* **Utility** – shows the unique supply point identifier of the site and details associated to the utility.
  * _Site (Parent)_ – this field shows the site name the utility is under and can be updated if a utility needs to be moved from one site to another via a dropdown list of available sites under the organisation.
  * _Identifier_ – this field shows the unique identifier of a supply point
  * _Commodity_
  * _Market Segment_
  * _Latest Retailer_
  * _Retailer Code_
  * _Commencement Date_
  * _Closure Date_
  * _Number of Network Access Points_
  * _Is Embedded Network_
  * _Do Not Monitor Missing Invoices_
  * _Utility Properties_
    * Network Tariff Code
    * Start Date
    * End Date
    * Transmission Loss Factor
    * Distribution Loss Factor
    *   Meter Count

