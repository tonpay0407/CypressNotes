# CypressNotes
- Notes on Cypress Automation
- Cypress directly interacts with browser, unlike selenium which interacts with browser via driver
- Javascript is used to write test cases
- Majorly used for websites written in angular, react, vue.
- Cypress test cases using Mocha framework (Mocha, Jasmine are frameworks are a unittest frameworks for javascript
- Multi browser testing can be used easily using test runner
- We can also run test cases via terminal instead of test runner - 
- npx cypress open or ./node_modules/.bin/cypress open - Command to open test runner
- npx cypress run - to run test cases via command prompt - running in headless mode
- npx cypress run --headed - to make the execution headed
- Running a single test case - node_modules\.bin\cypress run --spec "give path by copying test case's relative path"
- To run on a specific browser - node_modules\.bin\cypress run --browser chrome
- All commands are present in official docs of cypress - https://docs.cypress.io/guides/getting-started/writing-your-first-test#Write-your-first-test
	
Folder structure:
Test Data is maintained in fixtures folder
integration/examples - Test cases should be present here
plugins - containes events and listerns , example - if test case passed or failed and depending on which we need to perform some tasks
screenshots folder - screenshot will be saved here
support folder - resuable scripts are present here
videos folder - video files will be created here of our end to end test case
node_modules - contains libraries based on which cypress will work and will have mocha framework dependencies.
cypress.json file - we can overirde config settings. Default config settings are present in test runner - under settings tab
package.json - cypress dependency is added here

Locating Elements - 
cy.get(selector)
CSS selector we can write in different ways - .class

Tips:
Send keys in selenium == type in cypress
/// <reference types="Cypress" /> - Add thsi to get intellisense 
cypress get acts like find element
