# Organisation API

## General

The Organisation API is hosted at `<slug>.api.isg.zone`

## Public API

Prefixed with `public/`

Contains all the endpoints a user needs to get support. Supports authentication by BEARER tokens containing the users UUID or a jwt token to authentication a registered User

## Admin / Agent API

#### Agent API

Prefixed with `agent/`

Contains all the endpoints needed for agents to respond to tickets

#### Admin API

Prefixed with `admin/`

Contains all the endpoints needed for organisation admins to make changes to the organisation
