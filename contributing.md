# Contributing code
## [Github:](https://github.com)
Github is the codebase used for the Discipl project. There was a concious decision to use an open platform like Github over a closed git like Gitlab. This decision was made because the code of Discipl is open-source and has to be available to everyone who wants to develop for it.

#### -Project-board
Github's project board is a board where all the activities that happen within the team is stored. The board has collumns that indicate a fase for the user stories. In the collumns are the user stories that need to be done. When a user story has completed the fase which the collumn represents, the user story moves to the collumn on it's right. This is done till the user stories reach the collumn done, after which the user story is completed.

These user stories get compiled before and during the sprint meetings that happen at regular intervals. It's at this meetings that decisions about what user stories to handle at the current sprint occurs.

#### -pull request
Before edited code can be used on the master branche, a pull request needs to be made. This pull request will have the changes that are made to the code as opposed what is currently on the master branche. after 1 or more developers have approved of the changes, the changes can be implemented on the master branche.

#### -issues
When a (preceived) problem is detected in the code, an issue can be made. This issue will document the problem and make it visible to the team.

# Testing
## [Mocha:](https://mochajs.org/)
Mocha is a test executor. This package is in control of all the tests that are to be executed on the code. This framework works with tools like Sinon, Chai and Sonar that provide the actual tests for the code, and Mocha makes it possible to use "npm test" in the terminal and collectively execute the tests.

## [Chai:](https://www.chaijs.com/)
Chai is a framework that makes test conditions easy. Chai offers different APIs for BDD-testing. Our convention is to use the expect-variant. When one of the expects fails, it can be assumed that there was undefined behaviour.

## [Sinon:](https://sinonjs.org/)
To make the code reliable, multiple scenario's need to be tested. Sinon helps with that. It makes mock-databases, mock-entities, stubs and spies so this can be tested in a development enviroment, without using external tools like databases and/or filling databases with test data. This will ensure that all the scenario's that can be thought of in development will be tested if you run a test after making edits to the code.

## [Travis:](https://travis-ci.org/)
Travis is a continuous deployment platform. This program makes distributing changes in the code to working servers easier, run tests and perform code analysis. When changes are made and are accepted in Github, the changes are automatically rolled out to the servers that run on the software. Currently It's only used for tests and code analysis.

## [Sonar:](https://www.sonarsource.com/products/codeanalyzers/sonarjs.html)
Sonar is probably the best static code analyzer you can find on the market for JavaScript. Based on Sonarsource's JavaScript compiler front-end, it uses the most advanced techniques (pattern matching, dataflow analysis) to analyze code and find code smells, bugs and security vulnerabilities.

# Miscellaneous
## [Linter:](https://standardjs.com/)
In javascript (the language used for discipl) code can be formatted in multiple way's. while different company's use different standards for formatting their code, what the code does stays the same. Different developers use different formatting conventions which can make the code look sloppy if you see different style's in the same document. This is where Linter steps in. Linter inspects the code and formats it in such a way that it looks the same everywhere. Stuff like where the brackets get opened or closed, or if a space is used before using brackets, etc.

## Note on running code on older browsers
This project is made in ES6. This means that this program will not run on older browsers if the program is not converted to an older iteration of javascript. It is recommended to use [babel](https://babeljs.io/) to convert this code to a language that older browsers can understand if this program needs to be run on an older browser.
