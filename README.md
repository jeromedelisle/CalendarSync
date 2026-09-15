# CalendarSync

A single-file Microsoft 365 calendar viewer. Open `index.html` in a browser, configure an Entra app registration, and sign in to read your calendar through Microsoft Graph.

## Sign-in options

- **Browser sign-in (recommended):** uses the authorization-code flow with PKCE. Configure the page URL as a single-page application redirect URI and grant delegated `Calendars.Read`.
- **Username and password (legacy):** uses Microsoft Entra's resource-owner-password-credentials flow with the same application ID. This option is only available for a tenant-specific app with public client flows enabled; it does not support MFA or passwordless/federated sign-in. The password is submitted directly to Microsoft for the current session and is not stored by the page.
