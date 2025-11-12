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

# Users

Managing user access across an organization can be challenging without a clear system. The Users page solves this by giving admin users a central place to view, add, edit, or remove users. With detailed information on each account, admins can keep access secure and ensure the right people have the right permissions.

* **Email** – shows email address used to register a user
* **User status** – seen beside the email address to indicate the following which may require further action
* **Last Login** – shows date of latest login attempt for the user
*   **Role** – identifies which level of access is provided for the user (can only assign 1 per user)

    Highest to lowest permission level:

    * _EAX-Admin_
      * Has access to all organisations in Utilibox (this includes all the data tied to each organisation)
      * Has access to all EAX sections in Utilibox
    * _EAX-User_
      * Currently has no distinction from EAX-Admins but there are plans to add more difference in security settings in the future
    * _Channel-Partner_
      * Has access to selected organisations in Utilibox (this will only include the data tied to the selected organisation)
      * Does not have access to Reference Data, Meter Data, and Admin sections in EAX mode
    * _Company-Admin_
      * Has full access to only one organisation in Utilibox
    * _Company-User_
      * Similar to Company-Admins but will have some limited permission
      * Permissions not allowed:
        * Viewing of users under organisation
        * Inviting new users
        * Limiting access of other users to specific companies under the organisation
        * Viewing of LOAs
        * Creating or uploading of new LOA
        * Configuration of mailbox routes
    * _<mark style="color:$danger;">Signup-User – unavailable in User page</mark>_
      * _<mark style="color:$danger;">Entry level role for a user</mark>_
      * _<mark style="color:$danger;">No access to any organisation yet</mark>_
      * _<mark style="color:$danger;">Currently unused but previously for new users signing up for a Utilibox account</mark>_
* **Organisation** – lists the available companies a user has access to (can be multiple organisations for specific roles)
*   **Full Access** – a checkbox that allows users to activate/deactivate full access to specified organisation.

    * deactivate full access
    * activate full access – note that full access deactivates ability to choose organisation

    \*Change will only apply once you click on the save button
* **Actions** – allows the following administrative actions for the user
  * _Save profile_ - When successfully saved, a notification will show at the top of the screen
  * _More actions to manage account_
    * Resend account activation
    * Reset user authentication
    * Request password reset
    * Delete user



[adding-of-user.md](adding-of-user.md "mention")\
[editing-updating-user-profile.md](editing-updating-user-profile.md "mention")\
[deleting-of-user-profile.md](deleting-of-user-profile.md "mention")
