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



* Company – business name as shown in an invoice and is usually the listed name incorporated with the ABN
* Site – name of the site of the company but defaults to the address of the site unless otherwise specified
  * Company (Parent) – this field shows the company name the site is under and can be updated if a site needs to be moved from one company to another via a dropdown list of available companies under the organisation.
  * Site Name – this field shows the name of the site that is defaulted to the site address unless otherwise specified
  * Cost Code - this field shows the code for the site provided by the organisation when applicable.
  * Business Unit – this field shows the unit for the site provided by the organisation when applicable.
  * Site Code – this field shows the code for the site provided by the organisation when applicable.
  * Site Reference – this field shows the reference name for the site provided by the organisation when applicable.
* Address – shows the address of the site or business as listed in an invoice and can be setup to be the physical or billing address (or both) of the site.
  * Site (Parent) – this field shows the site name the address is under and can be updated if an address needs to be moved from one site to another via a dropdown list of available sites under the organisation.
  * Search for Address – this field allows for an automated search of an address using Google. User would only need to enter the address, and it automatically searches for the complete and correctly formatted address.
  * Formatted Address – this field shows the correct format and full address of a site based on the individual fields setup in the organisation tree.
  * Unit Number
  * Street
  * Suburb
  * State
  * Country
  * Postcode
  * Type – this field has a dropdown list that shows if an address is the physical or billing address of the site
  * Is Primary – if there are multiple addresses for a site, this can be enabled to determine if an address is their primary address.
* Utility – shows the unique supply point identifier of the site and details associated to the utility.
  * Site (Parent) – this field shows the site name the utility is under and can be updated if a utility needs to be moved from one site to another via a dropdown list of available sites under the organisation.
  * Identifier – this field shows the unique identifier of a supply point
  * Commodity
  * Market Segment
  * Latest Retailer
  * Retailer Code
  * Commencement Date
  * Closure Date
  * Number of Network Access Points
  * Is Embedded Network
  * Do Not Monitor Missing Invoices
  * Utility Properties
    * Network Tariff Code
    * Start Date
    * End Date
    * Transmission Loss Factor
    * Distribution Loss Factor
    *   Meter Count

