#### Milestones 

Milestones are an approach to where we can set expectations of what would make the software releasbile. It's a pretty general way of defining what is expected in a release. 

-----

### Milestone one


| Design Documents | Views/Controllers/Domain | Functionality | Database | Notification Server | Deployment | 
| --- | --- | --- | --- | --- | --- |
| First draft of the home page  | Domain: event (name, date, host, address, rsvp list) | User should be able to create an event (no authentication) | Create a database that fits the domain model (include script) | Plan out features and communication for notification server | None (this will use run-app to run) | 
| First draft of an event page   | Domain: Person (name, email, password)  | User should be able to view an event (no authentication needed) |  |  | f | 
| First draft of an create event page | View: Event Page |  |  |  |  | 
| First draft of an login page   | View: Create Event Page |  |  |  |  | 
| First draft of an registration page (not oauth)   | |  |  |  |  | 

### Milestone Two

| Design Documents | Views/Controllers/Domain | Functionality | Database | Notification Server | Deployment | 
| --- | --- | --- | --- | --- | --- |
| First Draft of an membership view for a group | Domain: event - description, how to contact us | Functionality | Database | Notification Server | Deployment | 
| First Draft of requesting membership to the group | Domain: Creation of member roles | Authentication works | Database | Create start of the server application | Setup jenkins to auto deploy on changes (test server) | 
| First Draft of group admins: role management | Controller: Can authenticate a user | Prevent non-authenticated users from creating events | Plan out how configuration is managed on the frontend and sent to the notifcation server  | | Auto bounce test site | 
| First Draft of oauth registration (filling in information gaps) |  |  |  |  |  | 


### Milestone Template

| Design Documents | Views/Controllers/Domain | Functionality | Database | Notification Server | Deployment | API |  
| --- | --- | --- | --- | --- | --- |
| Design Documents | Views/Controllers/Domain | Functionality | Database | Notification Server | Deployment | API | 
