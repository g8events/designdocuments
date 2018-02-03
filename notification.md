
## About 
The notification server is a communication channel agnostic server that is meant to pick up on events that are requested 
from the main server and will send out notifications to who their planned for and when they are planned for. Also, it is there 
to guarentee that a message was sent out if it missed the due date. 

## Expections 
 
  * This server is setup in isolation from the main server. 
  * 

## Communication 
  * Coming in: Via a JMS provider for instant requests 
  * Coming in: Rest Interface? (I'm not sure this is a great usage since the messages come in and the notification server isn't always guarenteed to be there.. jms queues can hold messages)
  * Going out: Information about what a notification syntax should fullfill. (Schema) Integrations can add extrafields or requirements 
  * Database: For messages that are queued up for later 
  * Going out: 
     * Individual integrations to customize the message based on it's channel
       * For example publishing on github may require a commit 
       * Publishing on twitter about the event may require a limit in characters 

  
## Features 
 * Should be able to send out a message or content body 
 * Handle a template for formating (in the case of email)
 * Handle the ability to opt out of emails (email integration and quick unsubscribe)
 * Handle the configuration for the server via remote configuration (the main server may be able to add in oauth connections)
 * Integrations are plug and play and can be added on at will 
 * Notications to be sent out can have a expiration and send-no-earlier than field 

 
## Nice to haves 
 * Log server support (Not sure what this means) 
 
## Suggestions for this

This is a good canidate for using Akka (and Probably Scala) since that it is there to be a high throughbput service, and is meant to handle failure gracefully.


------

One note: 

I am interested in seeing synconization of comments on the other oauthed platforms with the community. I.e. if a user comments on the reddit subreddit for the group you can see it from the event page, fb comments show up etc.
 