Continuous Integration (CI) is the practice of creating a smooth integration process on your software projects by continuously merging the developers' branches into the main branch. For this to work, we need to assert each merge's correctness before they can be integrated into the main repository, and for this, we use automated tests.   

This tutorial will go through the steps of setting up a pre-built Express application. This will then be used to set up automatic testing with `Jest` and `Supertest` and linting with `ESLint`, explaining the fundamentals of testing and linting in the process. See [this link](https://eslint.org/) for more information about Linting. Finally, we apply our newly acquired knowledge when we set up `Continuous Integration (CI)` with testing/linting using `GitHub Actions`.

#### Tutorial outline:
1. Background
2. Before you begin
3. Express application overview and set up
4. Automated integration testing for API endpoints with Jest and Supertest
5. Mocking the data model
6. Static code analysis with ESLint
7. Continuous Integration with GitHub Actions
8. Testing the GitHub Action

#### Prerequisites

This tutorial is aimed at users with basic programming knowledge, including JavaScript and GitHub.