# LITTLEPAY MERCHANT PORTAL

Littlepay is the world's only payment processor specializing in the transit and mobility sector. Public transit and mobility providers of all sizes use Littlepay's software and APIs to accept contactless and mobile payments.

## Node: 16.10.0 https://nodejs.org/en/

## NextJs: 12.3.1

## ReactJs: 18.2.0

## TailwindCSS: 3.1.8

### Table of contents
- [Setup](README.md#setup)
- [Run](README.md#run)
- [Build](README.md#build)
- [Tests](README.md#tests)
- [Prettier](README.md#prettier)
- [Update dependencies](README.md#update-dependencies)
- [Storybook](README.md#storybook)
- [Docker](README.md#docker)
- [Husky](README.md#husky)
- [I18Next](README.md#i18next)

### Setup
After you have Node.js installed on your system install Yarn through the npm package manager:
```
$ npm install --global yarn
```
We use yarn to manage the dependencies of the project:
```
$ yarn
```

### Configuration
Details about auth0 env variables needed (without the exact values) see examples here: [https://github.com/auth0/nextjs-auth0](https://github.com/auth0/nextjs-auth0#readme)

Use the following credentials to login into the project:

Username:

Password:

### Run
To run the project, use the following command:
```
$ yarn start
```

### Build
To build the solution, run the following command:
```
$ yarn build
```

### Tests
Tests are coded and run using `Jest`. (https://jestjs.io/ / https://testing-library.com/)

To run tests, run the following command:
```
$ yarn test
```

### Linting
`ESLint` is used as linting tool.

To run the lint run:
```
$ yarn lint
```

### Automation tests
Tests are coded and run using `Cypress`. (https://www.cypress.io/)

To run tests, run the following command:
```
$ yarn cy:run
```

### Prettier
Use `prettier` to format the code.

To format all code, run:
```
$ yarn prettier
```
To check if all the code is well-formated:
```
$ yarn prettier:diff
```

### Update dependencies
In order to support upgrading dependencies, we recommend to use:
```
$ yarn upgrade-interactive --latest
```

### Storybook
To individually test each component of the project, run the following command:
```
$ yarn storybook
```

### Docker

### Husky
Husky is used to lint the commit messages, run tests, lint code when you commit or push.

Documentation: https://typicode.github.io/husky/#/

### I18Next
I18Next is an internationalization-framework.

Documentation: https://www.i18next.com/
