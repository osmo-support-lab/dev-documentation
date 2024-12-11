# Message/Chat Status

### Chat

#### Status

* new
  * A new ticket that is not assigned/answered
* waiting\_for\_user
  * Agent has sent a message and now it's the users turn to answer
* waiting\_for\_agent
  * User answered and now it's the agents turn to answer
* delayed\_closing\*
  * Tickets with no interaction within 24hrs go into delayed closing and will close x (customisable) days afterwards
* on\_hold\*
  * Tickets that might need to be checked upon. A end\_time can be set on which the agent will get a reminder
* closed
  * Closed tickets -> no messages can be sent anymore

\* -> requires additional payloads (such as execution time)&#x20;

#### Status like attributes

* Action required (boolean)
  * Gets set by on-hold after the end\_time has been reached or if a non-assigned agent answers a ticket

### Message

A message has a status for the user and a status for the assigned agent.

#### Status

* sent
  * like Whatsapp one gray checkmark
* received
  * two gray checkmarks
* read
  * blue checkmark

###

