# TMKT-DLS-2.0


Feature: Login to DLS

Scenario: Login to admin view 
   Given : I login into DLS app 
   Then: I should see the "hands-on table" page with these columns  
   
      | Priority           | household ID     | Primary First Name     |  Primary Last Name   | Secondary Contact Full Name  | Phone 1   | Phone 2  | Email 1 |           | Email 2            | Street Address   | City                   | State                | Zip                          | RV Owner | Age       | Income       |       | Marital Status     | Program          | Marketing Participant  | Promotion            | Campaign Description         | Campaign Resort      | metaState           (State of the campaign)                  | Lead Date             | Assigned Agent       | Total Outbound Calls (pre-calc)       | Total Inbound Calls (pre-         calc)                | Total Inbound Calls      |  Total Live Calls (pre-calc)          | Latest Five9 disposition. 


 
Scenario: Admin needs to filter 
  Given: I apply filter on hands-on table 
  Then: The filter should be applied on all pages 
 


 

 
Scenario: Admin needs to change disposition 
   Given: I apply tour final disposition equals to no show  
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to no tour 
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to booked 
   Then: remove lead from hands on table 
   
   
   
   
   
 
   
   Scenario: Admin needs to change disposition 
   Given: I apply tour final disposition equals to no show  
   Then: add lead back to hands on table 

   
   
   
   
 Scenario: Admin can filter/sort all columns
 
 Given: I apply filter/sort on any columns
   Then: apply filter/sort on that column
   
   
      
 Scenario: Admin can assign one or more leads to agent
 
 Given: I need to assign multiple leads
 I can group or select multiple leads in the hands-on table via checkboxes
   Then: assign each row or selecting all in the current filtered view
   
 Given: I assign agent to a group of leads 
   Then: agent will be assigned to a group of leads
 
 Scenario:Leads should be sortedon priority basis
 Given: The leads have priority 1-5 assigned to them 
 Then: The leads should be sorted in hands-on table on priority 1-5
 
 Scenario: Admin can Assign priorities (the order in which the leads are called) order of leads in a list
 
 Given: I can assign priorities
   Then: I will be able to group or select multiple leads in the table via checkboxes against each row or selecting all in the current filtered view
   
 Given: I can assign priorities
   Then:  assign priorities to a group of leads
   
   Given: I can assign priorities  
   Then: I will able to sort leads
   
   
  Scenario: Admin should be able to filter via date

 Given:  Date range filter on top
   then: default it to the current year - date is by lead date







AGENT

Scenario: Login to Agent view 

   Given : I login into DLS app 
   Then: I can view the logged in agent's Assigned households only.
   
   
   
Scenario: Admin needs to change disposition 
   Given: I apply tour final disposition equals to no show  
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to no tour 
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to booked 
   Then: remove lead from hands on table 
   
   
   
   
   Scenario:  When a new lead for an already assigned lead is ingested 
   
   Given: I see new lead for an already assigned lead is ingested 
   Then:  It should also show up under the same household which was already assigned to the user
   
   
   
   Scenario:  Leads listed in priority
   
   Given:  Leads are grouped and listed in order of priority 1 - 5
   Then:  Agents cannot change their sort order
   
   
   
   
     Scenario: Phoen number are clickable
   
   Given: The phone numbers in the table are clickable
   Then:  Agent clicks phone to call
   


   
   Scenario:  Agent clicks to phone call
   
   Given: Agent clicks phone to call
   Then:  Call is opened in Five9 HTML Web


  
  Scenario:  Call is opened in Five9 HTML Web
   
   Given: Call is opened in Five9 HTML Web
   Then:  Call opens household in Engage connector



  Scenario:  Agent actions
   
   Given: Agents cannot change assignments or priority
   Then:  Agents can filter
   
   


   
   
   
   
   
   
