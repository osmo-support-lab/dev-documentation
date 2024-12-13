# Authentication

## General

As defined in the DatabaseModels the API supports two types of users:

* Anonymous Users
* Users

## Anonymous Users

A anonymous user is a user who seeks support through the widget. Every time the widget is opened for the first time the user shall get registered. The registration is done through the Organisation API as a anonymous user is tied to an organisation.&#x20;

### Authentication

The anonymous user is authenticated through the UUID. Once he looses his UUID (e.g. cleared cookies, cookie expired, new browser) the user will get registered again.&#x20;

The user can connect his email to the anonymous account. In such case he can then restore previous conversations. This is a feature that is not part of v1.

## User

A user is a system wide account and is not tied to an organisation. It is mainly used for agents/organisation admins.

A user can belong to multiple organisations and have various roles. The exact role mechanism is described in "Roles & Permissions"

### Authentication

The user is authenticated through email and password. The backend will then issue a jwt token.
