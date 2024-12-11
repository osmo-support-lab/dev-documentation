# Overview

## Idea

The idea is that every request which changes the internal state (new message, status change, etc.) triggers a  event which gets dispatched to subscribers. This will allow us to modularily extend the features and implement more workflows, integrations, etc.\
\
The webhooks, websockets and also the automations will be built upon these events.

## Implementation

The Event manager will be the central place. It should allow a modular approach to event handling. Modules can register their event handlers which will get dispatched on the event. Error handling is up to the event handler. The event manager will catch all exceptions and continue the workflow.&#x20;

**Note: Critical operations such as inserting the initial data to the database should NOT be handled as module as a module can't make a call fail. If it fails it will be skipped.**

It supports the following functions:

* register(events: list, check\_func: function)
  * Registers a new event handler that will get triggered if the check\_func callback returns true
* dispatch(event: str, payload: dict)
  * Dispatches a event to all registered event handles for the event
  * Checks whether event id matches and the registered check\_fund returns true

## Implemented Handler

The next pages in this section will contain all created event handlers and a description of what they do.

