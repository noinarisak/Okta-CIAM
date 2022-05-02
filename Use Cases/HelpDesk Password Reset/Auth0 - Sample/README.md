# HelpDesk Password Reset Tool (Auth0)

This app implements a sample HelpDesk Password Reset tool.

![HelpDesk Password Reset](public/images/HelpDeskPasswordReset.png)

## Setup

* Get a management API token manually for testing - [Instructions here](https://auth0.com/docs/secure/tokens/access-tokens/management-api-access-tokens)

* Create a regular web application

* Enable **email** Passwordless connection. Add the web application created to the connection.

* Ensure test user profile has the following metadata -

```
{
  "telephone": <Phone Number>,
  "address": <Address data>
}

```