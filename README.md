# LITTLEPAY MERCHANT PORTAL

Littlepay is the world's only payment processor specializing in the transit and mobility sector. Public transit and mobility providers of all sizes use Littlepay's software and APIs to accept contactless and mobile payments.

## Node: 16.10.0

## NextJs: 12.3.1

## ReactJs: 18.2.0

### Table of contents
- [Setup](README.md#setup)
- [Run](README.md#run)
- [Build](README.md#build)
- [Tests](README.md#tests)
- [Prettier](README.md#prettier)
- [Update dependencies](README.md#update-dependencies)

### Setup
We use yarn to manage the dependencies of the project:
```
$ yarn
```

### Configuration
Details about auth0 env variables needed (without the exact values) see examples here: [https://github.com/auth0/nextjs-auth0](https://github.com/auth0/nextjs-auth0#readme)

### Run
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
