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

# Adding of User

1. On the upper right-hand side of the page, click on the "Invite User" button, a pop-up window will appear.
2. On the email section, enter the email address of users to be added (when adding multiple users, separate the email address with a semicolon).
3. Choose the role of the users to be added.\
   Roles ordered by highest to lowest permission level:
   * EAX-Admin
     * Has access to all organisations in Utilibox (this includes all the data tied to each organisation)
     * Has access to all EAX sections in Utilibox
   * EAX-User
     * Currently has no distinction from EAX-Admins but there are plans to add more difference in security settings in the future
   * Channel-Partner
     * Has access to selected organisations in Utilibox (this will only include the data tied to the selected organisation)
     * Does not have access to Reference Data, Meter Data, and Admin sections in EAX mode
   * Company-Admin
     * Has full access to only one organisation in Utilibox
   * Company-User
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
4.  Choose the organisation where user would need access to.

    _Note: Only EAX users and Channel Partner roles are allowed to have access to multiple organisations which can be done in the main users page._
5. Click Invite once done. A notification will show indicating that the user has been successfully added.
6. The user should receive a confirmation email to activate their Utilibox account.
7. User can click the “Click here to activate your account” button or copy the link provided.
8. User will be directed to a page where they can set their password. Once done click on “Set Password”.
9. User will then be asked to set up multi-factor authentication. Follow the instructions indicated on the page to continue with the account activation.
10. Upon successful activation, user will be directed to the login page of Utilibox where they can enter their newly setup username (email) and password.
