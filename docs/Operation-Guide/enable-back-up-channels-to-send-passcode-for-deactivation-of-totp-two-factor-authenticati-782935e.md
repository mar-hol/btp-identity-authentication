<!-- loio782935ec3c904178837e96043f2bbc6f -->

# Enable Back-Up Channels to Send Passcode for Deactivation of TOTP Two-Factor Authentication Devices

Tenant administrator can configure back-up channels to send TOTP deactivation passcodes to the user.



<a name="loio782935ec3c904178837e96043f2bbc6f__prereq_lrj_kvs_rjb"/>

## Prerequisites

-   You are assigned the *Manage Tenant Configuration* role. For more information about how to assign administrator roles, see [Edit Administrator Authorizations](edit-administrator-authorizations-86ee374.md).

-   \(for the SMS channel\) The user must have a verified phone.

-   \(for the SMS channel\) You have configured the Sinch Service option in the administration console for Identity Authentication. For more information, see [Configure Sinch Service in Administration Console](configure-sinch-service-in-administration-console-f4a04ed.md).

-   \(for the e-mail channel\) The user must have a verified e-mail address.

-   \(for the e-mail channel\) You have configured an e-mail template for the *Deactivate TOTP Device* process. For more information, see [Configuring E-Mail Templates](configuring-e-mail-templates-b2afbcd.md).

    > ### Remember:  
    > The *$\{other.totpResetPasscode\}* parameter is mandatory for the *Deactivate TOTP Device* template.




## Context

The primary channel to deactivate a device is the passcode generated by the mobile device. If no other back-up channel is enabled, this option is the only one for the user in the *Two-Factor Authentication* section of the administration console for Identity Authentication.

When the back-up channels, *SMS* and/or *E-Mail* are enabled in the administration console, the user can choose from the options on the profile page: *TOTP Passcode*, *Passcode via SMS*, and *Passcode via E-Mail*.

> ### Remember:  
> It takes 2 minutes for the configuration changes to take place.

To enable or disable back-up channels for deactivation passcode, follow the procedure below:



## Procedure

1.  Access the tenant's administration console for Identity Authentication by using the console's URL.

    > ### Note:  
    > The URL has the following pattern:
    > 
    > `https://<tenant ID>.accounts.ondemand.com/admin`
    > 
    > *Tenant ID* is an automatically generated ID by the system. The first administrator created for the tenant receives an activation e-mail with a URL in it. This URL contains the *tenant ID*. For more information about your tenants, see [Viewing Assigned Tenants and Administrators](../viewing-assigned-tenants-and-administrators-f56e6f2.md).
    > 
    > If you have a configured custom domain, the URL has the following pattern: `<your custom domain>/admin`.

2.  Under *Applications and Resources*, choose the *Tenant Settings* tile.

    At the top of the page you can view the administrative and license relevant information of the tenant.

3.  Choose the *Multi-Factor Authentication* list item.

4.  Under *TOTP Deactivation Passcode Channels Configuration*, enable or disable the options according to your needs.

    -   *SMS*
    -   *E-Mail*

    If the operation is successful, the system displays the message ***TOTP Deactivation Options updated***.




<a name="loio782935ec3c904178837e96043f2bbc6f__result_mqz_lwh_h3b"/>

## Results

Users can choose from the back-up channel options on their profile page if they are enabled via the administration console.

If no option is enabled, the users do not see the radio buttons on their profile page.

**Related Information**  


[Tenant SAML 2.0 Configuration](tenant-saml-2-0-configuration-e81a19b.md "You as a tenant administrator can view and download the tenant SAML 2.0 metadata. You can also change the name format and update your certificate used by the identity provider to digitally sign the messages for the applications.")

[Tenant OpenID Connect Configurations](tenant-openid-connect-configurations-3d6abcc.md "You as a tenant administrator can view and configure the tenant OpenID Connect configurations.")

[Change Tenant Texts Via Administration Console](change-tenant-texts-via-administration-console-c24b1d0.md "The change tenant texts option can be used to change the predefined texts and messages for end-user screens available per tenant in Identity Authentication via the administration console.")

[Configure Master Data Texts Via Administration Console](configure-master-data-texts-via-administration-console-c068ac9.md "The master data texts option can be used to configure the predefined master data for each resource in Identity Authentication via the administration console.")

[Configure Links Section on Sign-In Screen](configure-links-section-on-sign-in-screen-060c032.md "You can configure links to appear on the sign-in screen of your applications.")

[Add Instructions Section on Sign-In Screen](add-instructions-section-on-sign-in-screen-c9e717e.md "You can customize the sign-in sscreen of the Horizon theme with instructions for the user.")

[Configure X.509 Client Certificates for User Authentication](configure-x-509-client-certificates-for-user-authentication-52c7dcb.md "Tenant administrators can configure X.509 client certificates for user authentication as an alternative to authenticating with a user name and a password.")

[Configure Tenant Images](configure-tenant-images-8742046.md "You can configure a custom global logo and, or a background image on the forms for sign-in in, registration, upgrade, password update, and account activation for all applications in a tenant. You can also set a favicon for tenant.")

[Configure Allowed Logon Identifiers](configure-allowed-logon-identifiers-3adf1ff.md "Tenant administrators can choose the allowed logon identifiers for the users.")

[Configure User Identifier Attributes](configure-user-identifier-attributes-8b9fa88.md "Tenant administrators can configure user identifier attributes as required and unique for the tenant.")

[Configure Trust this browser Option](configure-trust-this-browser-option-5b8377e.md "Tenant administrator can set the number of days for which the users won't get prompted for second-factor authentication, if they sign in from the same browser.")

[Enable Users to Recover Password with Security Questions](enable-users-to-recover-password-with-security-questions-d9ae898.md "Users can choose to answer security questions to reset their password.")

[Enable Users to Recover Password with PIN Code](enable-users-to-recover-password-with-pin-code-046a235.md "Users can choose to provide PIN code to reset their password.")

[Configure Initial Password and E-Mail Link Validity](configure-initial-password-and-e-mail-link-validity-f8093f4.md "As a tenant administrator, you can configure the validity of the initial password and link sent to a user in the various application processes.")

[Configure Session Timeout](configure-session-timeout-5ca23e4.md "As a tenant administrator, you can configure when the session, created at the Identity Authentication tenant, expires.")

[Configure Trusted Domains](configure-trusted-domains-08fa1fe.md "Service providers that delegate authentication to Identity Authentication can protect their applications when using embedded frames, also called overlays, or when allowing user self-registration.")

[Use Custom Domain in Identity Authentication](use-custom-domain-in-identity-authentication-c4db840.md "Identity Authentication allows you to use a custom domain that is different from the default one (<tenant ID>.accounts.ondemand.com) - for example www.mytenant.com.")

[Change a Tenant's Display Name](change-a-tenant-s-display-name-a513c91.md "You can configure the tenant's name from the administration console for Identity Authentication.")

[Configure Default Risk-Based Authentication for All Applications in the Tenant](configure-default-risk-based-authentication-for-all-applications-in-the-tenant-1aab51a.md#loio1aab51ae62b94f79b4c6dac7a00857c2 "You can define rules for authentication according to different risk factors and apply actions like Allow, Deny, and Two-Factor Authentication for all applications in a tenant.")

[Configure Sinch Service in Administration Console](configure-sinch-service-in-administration-console-3fdc9e1.md "Configure Sinch Service to enable Phone Verification via SMS or SMS Two-Factor Authentication in the administration console.")

[Configure RADIUS Server Settings \(Beta\)](configure-radius-server-settings-beta-03043ae.md "Configure Remote Authentication Dial-In User Service (RADIUS) server settings in the administration console for Identity Authentication.")

[Configure Mail Server for Application Processes](configure-mail-server-for-application-processes-ccc7ba1.md "Configure mail server for the e-mails sent to the end users in the different application processes.")

[Configure IdP-Initiated SSO](configure-idp-initiated-sso-5d59caa.md)

[Send Security Alert E-Mails](send-security-alert-e-mails-c977464.md "Send security alert e-mails to end-users or administrators when changes in their accounts are made.")

[Send System Notifications via E-Mails](send-system-notifications-via-e-mails-aa04a8b.md "You can configure the administration console to send e-mails with information about expiring certificates, system notifications and new administrators to specific e-mail addresses or to the e-mails of all administrators.")

[Configure Default Language for End User Screens](configure-default-language-for-end-user-screens-2cb73c3.md "Select the language that the end user screen uses if the language of the browser isn’t in the list of supported languages.")

[Configure P-User Next Index](configure-p-user-next-index-045bb1c.md "Set the value for the P-user next index.")

[Reuse Identity Authentication Tenants for Different Customer IDs](reuse-identity-authentication-tenants-for-different-customer-ids-ebd0258.md "You as a tenant administrator can reuse an existing tenant for configurations and automated subscriptions.")

