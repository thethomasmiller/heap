# heap

# Data Model
                  ________ Account________
        ____User____                 ____User____
    Session       Session          Session      Session 
    Pageview      Pageview         Pageview     Pageveiw
    Events        Events           Events       Events 

# Properties: 
bits of metadata from user interactions.
Classified based on their place in the data model

   # User-Level properties: 
   all attributes associated with a user, including touch properties, account information, business logic, and more. Apply across the entire hierarchy. 

   # Session-level properties:
   all attributes captured at the session level, such as the landing page, browser, referrer, and more. Session properties trickle down and exist at the event level. 

   # Pageview-level properties:
   all attributes associated with a particular pageview (or screenview on native mobile sdks) such as path, title, and domain. Snapshots created on pageview events will result in pageview-level properties, and these properties will trickle down to all events that occur on that page. 

   # Event-level properties: 
   all attributes associated with events including, last touch properties, target text or context captured by snapshots, such as price or quantity. 
   Custom events can be created, aka events sent out via Heap track APIs, to have additional metadata(SKU, Email Subject, Successful Charge etc.) associated with your user interactions. 

   Event level properties only apply to those specific events. When grouping by event-level properties you have to select the event with the properties you would like to group by. 

# First Touch Properties vs. Last Touch Properties 

In addition to the property types above, Heap distinguishes between first touch and last touch properties based on when the interaction occurred in relation to the history of the user. Whether a property is *first touch*, *last touch*, or somewhere in between plays a role in how it fits into the data model.


### AUTOCAPTURE

# EVENTS 
View page: A pageview 
Click on: A click on an element 
Change on: A change in an input, textarea, or select element 
Submit on: A form submission 
Start Session: A session

# USER PROPERTIES


Mock Implementation

Demonstrate that you understand the basics of Heap's data model, APIs, and how customers can use data within the tool to answer business questions. 

1) Identify all the data sources that the client can bring into Heap (usage data, payment data, email data etc)

identify API






2) Explain how to map all of these different sources of data to our data model and how to leverage our APIs to do so. 

3) Explain how you'd be able to use this data set to answer specific analysis questions in the context of Heap. 

