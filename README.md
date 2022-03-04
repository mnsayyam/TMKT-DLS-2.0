# TMKT-DLS-2.0


Feature: Login to DLS

Scenario: Login to admin view 
   Given : I login into DLS app 
   Then: I should see the "hands-on table" page which have these columns  
   Given I have the following household with given information
      | Priority           | household ID     | Primary First Name     |  Primary Last Name   | Secondary Contact Full Name  | Phone 1   | Phone 2  | Email 1 |           | Email 2            | Street Address   | City                   | State                | Zip                          | RV Owner | Age       | Income       |       | Marital Status     | Program          | Marketing Participant  | Promotion            | Campaign Description         | Campaign Resort      | metaState           (State of the campaign)                  | Lead Date             | Assigned Agent       | Total Outbound Calls (pre-calc)       | Total Inbound Calls (pre-         calc)                | Total Inbound Calls      |  Total Live Calls (pre-calc)          | Latest Five9 disposition. 


 
Scenario: Admin needs to filter 
  Given: I apply filter on hands-on table 
  Then: The filter should be applied on all pages 
 

 
Scenario: Admin needs Server-side Pagination 
  Given: I apply server-side pagination on hands-on table 
  Then: The server-side pagination should be applied on all pages 
 

 
Scenario: Admin needs to change disposition 
   Given: I apply tour final disposition equals to no show  
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to no tour 
   Then: add lead back to hands on table 

   Given: I apply tour final disposition equals to booked 
   Then: remove lead from hands on table 
