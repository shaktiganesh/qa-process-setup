# qa-process-setup

## Where would you start?What would be your first steps?
  Assuming the REST API is a separate micro service and is part of the cross functional team for which the QA process is to be established,
  
 Initial steps would be to come up with a high level test strategy and test plans to test the front end application and REST API independently and integration between the two.
  
 In which few of the important factors to be considered are 
 
● Analyse overall QA scope, recruitment of testers (if needed based on skillset) ,integration of QA early in the workflow

● Effective communication between cross functional teams(show and tell with PO etc), QA to gain the maximum functional    
knowledge

● Tools,scope for early/in sprint automation, define test scope, test cases/scripts 

● QA environments to be setup

● Frameworks, language

● CI/CD pipeline

● Test management, reporting

## Which process would you establish around testing new functionality? How would you want the features to be tested

For the REST API,

● TDD + BDD approach to add new functionalities and test them to the product

● Good to have the unit tests(by dev) and the automated behavior tests(by QA team) in the same code base to enable continous    delivery smoothly

● New features to be tested will be added as the automated behavior tests within the same sprint by QA team

● QA workflow in the sprint- grooming/planning,develop automated behavior tests/run test suite, defect management, QA sign off

● 100% automation of the new features in the same sprint should be feasible for the REST API tests.

● Sample automation for rest services https://github.com/shaktiganesh/restapi-testing

For the front end application

● Combination of Manual testing + Automation in the sprint for new functionalities.(However in sprint automation should be discussed with cross functional teams mainly with PO, to see how changing, the requirement scope is in the future. Ideally in sprint automation could be adopted after the product development reaches certain stability and not from very start)

● Manual team -to test the new functionalities manually within the sprint

● Product Owner’s user stories(good to have in Gherkin) format to be the base for manual testing.

● Automation team-to develop In sprint automation for the user stories in the current sprint. 

● The automation scripts for the user stories of the current sprint to be used as regression scripts for n+1 sprint.

 Integration testing plan also to be made for testing the REST API  releases (version x with n new functionality )
 with front end application releases (version y with n new functionality)
 
 ## Which tools would you suggest using to help your team with a daily work?
 
● Gherkin - Product owner/QA

● Cucumber - Develop step definitions (automated  behavior tests)

● Rest Assured -Framework to test REST API

● Selenium- Framework to test front end application

● Atlassian suites(JIRA, CONFLUENCE, BITBUCKET, BAMBOO) to support Agile process, methodologies and CI/CD
 
 ## If you would do a test automation which techniques or best practices would you use the application?
 
● Framework to suit the application needs, eg. Data Provider in TestNG to be used for heavy data driven application

● Early automation as possible with right tool selection

● In sprint automation if feasible (No manual regressions, if this is achieved)

● Including the automation team to planning sessions to get depth of the functionalities (important for inspirit automation)

● Continuous integration of tests

● Automation code in the same code base as developer if feasible to enable continuous delivery

● Tests naming should be closely precise to what the test does

● Automate first the test cases used frequently and the hard to manually test, test cases

● Be informed early about the front end changes from the developer team and stress using 'id' as the identifier for web applications as much as possible

● Creation of effective test data that could be resuable


