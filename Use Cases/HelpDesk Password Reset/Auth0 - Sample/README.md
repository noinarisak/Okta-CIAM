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

## Sample application

* From a Glitch account remix the following app - https://glitch.com/edit/#!/hdauthotool

* Create a **.env** file at top level, if not already there

* Add the following values to the **.env** file -

```
BASE_URL: https://<your auth0 tenant>
CLIENT_ID: <Client ID of the web application>
CLIENT_SECRET: <Client Secret of the web application>
CONNECTION: <Auth0 database Connection the user is in>
API_TOKEN: <management API token>

```

* Access the application through preview