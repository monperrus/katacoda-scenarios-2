*This step introduces GitHub Actions, Automated integration testing in JavaScript using Jest and Supertest, and static code analysis using ESLint. If you are already familiar with these concepts, you can jump to the next step.*

#### Github Actions

Github Actions is a tool that can run automated scripts on specific events on Github like push or pull requests. With Github Actions, we can easily set up a CI/CD environment to automate our Software workflow by building, testing, and deploying our code right in Github. In this tutorial, we will cover how to set up a CI workflow, but GitHub Actions could as well be used for Continuous Deployment (CD). [More info.💬](https://docs.github.com/en/actions)

#### Integration testing in Javascript

Testing API endpoints often includes testing multiple functions that span across various pieces of the application. This sort of testing is called integration testing and will be used throughout this tutorial. We will write such tests using the JavaScript framework Jest and the module Supertest. [More info.💬](https://en.wikipedia.org/wiki/Integration_testing)

##### Jest

Jest is a JavaScript testing framework that enables users to write automated tests for JavaScript projects. The framework has had great success because of its minimal demands on configuration and its extensive and well-documented API. Jest is compatible with several well-known JavaScript frameworks such as TypeScript, Node, React, Angular and Vue. [More info.💬](https://jestjs.io//)

##### Supertest

Supertest is a JavaScript module that enables us to send HTTP requests to test API endpoints. It provides a high-level abstraction for testing HTTP while easy to use. [More info.💬](https://www.npmjs.com/package/supertest)

##### Mocking with Jest

Mocks provide the capability to abstract the behaviour of a functional dependency while testing. This technique is beneficial when making HTTP calls to an API or interacting with the database layer/data model. 

This tutorial will utilize mocking to abstract the data model. Doing so empowers us to perform API endpoints testing without interaction with the actual data model. This means that HTTP requests from the written tests do not interact with the existing data model in `models/Todos.js`. Instead, we use mock data defined in the test file. Even though we only use a simple data model to store non-persistent data in this application, we could use the same technique when an actual database is apparent. [More info.💬](https://jestjs.io/docs/mock-function-api)

#### Static code analysis with ESLint

ESLint is a static code analysis tool used to find bugs, programming errors, and code formatting errors. This process of finding these types of errors is called *Linting*. It is built into most text editors and is suitable to run as part of the CI pipeline. The tool also offers automatic syntax-aware error fixes for many problems that automatically resolve bugs and errors. [More info.💬](https://eslint.org/)