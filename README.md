# Project-Burn-Chart-Revision
A summary of revision for the Burn Chart by Michael Burnett

OVERVIEW
1.	Project Background and Description
  This project is intended to replace the current “Project Burn Chart” processes.  In this processes Danielle uses data from a spread     sheet to gather the number of our spent on projects and present the data internally as well as externally.  The spread sheet receives   its data from a sql data base that has the time that project contributors have spent on the project. 
2.	Project Scope
  The scope the project is only to replace the portion of the excel spread sheet that deal with the number of hours on the project. This  project is limited to 100-150hrs. 
3.	High-Level Requirements
    The new application must include the following:
      •	Ability to create a report similar to the one in excel that shows worked vs. approved hours
      •	Ability to be accessed both within the company network and outside of the company network
      •	Ability to create a .msg that contains the report. 
      •	Ability to record both internal and external comments
    The new application should:
      •	Be easy to use
      •	Follow established coding standards
      •	Make the processes of delivering this data to the client and internal stake holders easier.
4.	Details to Track
    •	Time is currently held in a sql database. 
    •	New stored procedures may be needed to pull data. 
    •	Internal Website hosting is available. 
    •	SSRS is available. 
    •	A new resource (intern) is starting soon. 
    •	Internal Tool with External Access.
    •	Data is delivered in the body of the email. 
    •	New ability to stored concerns. 
    •	Secure application internal users only.
5.	Deliverables
      A high quality easily maintainable web application accessible internally or externally. 
6.	Specific Exclusions from Scope
      It is not to include (at this time) the different tabs that further aggregate the data.  
7.	Technical
      New Data Table: Case_Concerns
      In order to sore the Data related to case concerns a new data table may be needed:
      Case_Concerns
      RowId (int) (pk)
      CaseId (varchar) (fk)
      Concern (varchar)
      Internal (bool)
      ConcernDate (datetime)
      Resolved (bool)

8.	Research
  Create an outlook mail message:
http://stackoverflow.com/questions/6848789/create-open-existing-msg-from-path-to-new-outlook-mailitem-in-c-sharp
  SSRS HTML 5 Support
https://social.technet.microsoft.com/Forums/sqlserver/en-US/13f0214c-6f8d-4860-8ef7-995eed4a6f6b/viewing-ssrs-reports-in-html5



