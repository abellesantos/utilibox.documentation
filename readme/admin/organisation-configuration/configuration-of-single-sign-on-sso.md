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
  tags:
    visible: true
---

# Configuration of Single Sign‑On (SSO)

Utilibox supports enterprise Single Sign‑On (SSO) using industry‑standard SAML 2.0, allowing your organisation to manage user access securely through your existing identity provider (such as Microsoft)

Setting up SSO is a straightforward three‑step process, outlined below.

<figure><img src="../../../.gitbook/assets/SSO Setup.png" alt=""><figcaption></figcaption></figure>

### Confirm Your Email Domain

To enable SSO, Utilibox must first verify that you own the email domain used by your organisation.

1. In Utilibox, go to Admin > Organisation Configuration > Security and click on "Enable SSO"
2. Enter your organisation’s domain in the **Add Email Domain** field.
3. Click **Add**.
4. You’ll be provided with a **TXT record**. Copy this record into your domain’s DNS configuration.
5. Once the TXT record has been added, return to Utilibox and click **Verify** next to your domain.

> **Note:** DNS changes can take time to propagate. If verification does not succeed immediately, wait a short while and try again.

### Configure Your Identity Provider Using Utilibox Information

Next, you’ll set up an enterprise application in your SAML identity provider using details provided by Utilibox.

1. In your identity provider (for example, Microsoft Entra ID), create a new **Enterprise Application** for Utilibox.
2. In Utilibox, copy the **Identifier / Entity ID** and paste it into the corresponding field in your identity provider.
3. Copy the **Reply URL** from Utilibox and enter it into the matching field in your identity provider.

These values allow your identity provider to trust and communicate securely with Utilibox.

### Configure Utilibox Using Your Identity Provider Information

Finally, you’ll return to Utilibox and enter information from your identity provider.

1. Copy the **Login URL** from your identity provider and paste it into the **Login** field in Utilibox.
2. Copy the **Identity Provider Entity ID** and paste it into the corresponding field in Utilibox.
3. Download the **signing certificate** from your identity provider and upload it into Utilibox.

### Test and Finalise

1. **Save** your configuration.
2. Test SSO to confirm users can sign in successfully using your identity provider.

Once you are confident that SSO is working correctly, you can disable **Allow Password Fallback**.\
This ensures users can **only sign in via SSO**, further strengthening your organisation’s security.

***

### Need Help?

If you encounter any issues during setup, our support team can help guide you through the process or validate your configuration.
