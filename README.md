# qa-process-setup

## Where would you start?What would be your first steps?
  Assuming the REST API is a separate micro service and is part of the cross functional team for which the QA process is to be established,
  
 Initial steps would be to come up with a high level test strategy and test plans to test the front end application and REST API  independently and integration between the two.
  
 In which few of the important factors to be considered are 
1)Analyse overall QA scope, recruitment of testers (if needed based on skillset) ,integration of QA early in the workflow
2)Effective communication between cross functional teams(show and tell with PO etc), QA to gain the maximum functional    knowledge
3)Tools,scope for early/in sprint automation, define test scope, test cases/scripts 
4)QA environments to be setup
5)Frameworks, language
6)CI/CD pipeline
7)Test management, reporting

## Which process would you establish around testing new functionality? How would you want the features to be tested

For the REST API,
- TDD + BDD approach 
-Good to have the unit tests(by dev) and the automated behavior tests(by QA team) in the same code base. 
-New features to be tested will be added as the automated behavior tests within the same sprint by QA team
-QA workflow - grooming/planning , develop automated behavior tests/run test suite, defect management, QA sign off
-100% automation should be feasible for the REST API tests.

For the front end application
-Combination of Manual testing + Automation in the sprint
-Manual team -to test the new functionalities manually within the sprint
-Product Owner’s user stories(good to have in Gherkin) format to be the base for manual testing.
-Automation team-to develop In sprint automation for the user stories in the current sprint. 
-The automation scripts for the user stories of the current sprint to be used as regression scripts for n+1 sprint.

 Integration testing plan also to be made for testing the REST API  releases (version x with n new functionality )
 with front end application releases (version y with n new functionality)
 
 ## Which tools would you suggest using to help your team with a daily work?
 Gherkin - Product owner/QA
 Cucumber - Develop step definitions (automated  behavior tests)
 Rest Assured -Framework to test REST API
 Selenium- Framework to test front end application
 Atlassian suites(JIRA, CONFLUENCE, BITBUCKET, BAMBOO) to support Agile process, methodologies and CI/CD
 
 ## If you would do a test automation which techniques or best practices would you use the application?
 -Framework to suit the application needs
 -Early automation as possible
 -In sprint automation 
 -Including the automation team to planning sessions to get depth of the functionalities (important for inspirit automation)
