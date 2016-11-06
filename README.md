# Documentation
Archetecture.md describes the project archetecture and design principles.
FullUML.png and SimplifiedUML.png give project UML diagrams
FrameworkDocumentation.md describes the frameworks on which the application is built and why they were chosen
Dev-Process.md details our development process
Feature List.md lists all existing features of the application and further describes them

## Problem Statement
Many currently marketed home and business finanace and accounting programs are insufficent in that they are not tailored to be flexible enough to meet all the needs of their clients, or that they are forcing a feature that isn't essential to the clients' needs. Our goal is to develop an easy to use, flexible application that will satisfactorily handle the client's finance and accounting related tasks.

We have received the following features to implement from our client
* Ability to import financial transaction records from extern sources (i.e. a bank
  or other financial management software)
* Ability to manually add individual transaction records
* Encryption of data both in-memory and on the disk
* The ability to scan all financial records and identify duplicate transactions
* Generate a set of charts/metrics in order to analyze financial history and trends
* A financial management system - The ability to create a budget and account for
  things such as recurring bill payments
* Ability to tag and categorize individual transactions so that the user can more
  easily search and filter transactions
* The System should be able to automatically suggest tags for imported payments


#Development Systems
## IDE
[Jetbrains] Java IDE named [IDEA]

## Workflow Tracking
We use [JIRA] to track our workflow.

## Continous Integration
We use [Travis] for Continous Integration. All our teams repos can be found at [Travis-Ledger]





[Jetbrains]:                          https://www.jetbrains.com/
[IDEA]:                               https://www.jetbrains.com/idea/
[Travis]:                             https://travis-ci.org/
[Travis-Ledger]:                      https://travis-ci.org/Ledger-Software/
[JIRA]:                               http://cjm721.com:8080/secure/RapidBoard.jspa
