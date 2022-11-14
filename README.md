# LITTLEPAY MERCHANT PORTAL

Littlepay is the world's only payment processor specializing in the transit and mobility sector. Public transit and mobility providers of all sizes use Littlepay's software and APIs to accept contactless and mobile payments.

### Table of contents
- [Setup](README.md#setup)
- [Build](README.md#build)
- [Run](README.md#run)
- [Prettier](README.md#prettier)
- [Linting](README.md#linting)
- [Unit tests](README.md#unit-tests)
- [Automation tests](README.md#automation-tests)
- [Update dependencies](README.md#update-dependencies)
- [Storybook](README.md#storybook)
- [Docker](README.md#docker)

### Setup
First step is to install Node.js on your system: https://nodejs.org/en/

After you have Node.js installed on your system install Yarn through the npm package manager:
```
$ npm install --global yarn
```
We use yarn to manage the dependencies of the project:
```
$ yarn
```

The project uses the following tooling versions:
- **Node**: `16.10.0`
- **Typescript**: `4.8.3`
- **NextJs**: `12.3.1`
- **ReactJs**: `18.2.0`
- **TailwindCSS**: `3.1.8`

#### **Husky**
Husky is used to lint the commit messages, run tests, lint code when you commit or push.

Documentation: https://typicode.github.io/husky/#/

#### **I18Next**
I18Next is an internationalization-framework. It provides a complete solution to localize your product from web to mobile and desktop.

Documentation: https://www.i18next.com/

### Configuration
Details about auth0 env variables needed (without the exact values) see examples here: [https://github.com/auth0/nextjs-auth0](https://github.com/auth0/nextjs-auth0#readme)

### Build
To build the application for production usage, run the following command:
```
$ yarn build
```

### Run
To start a Next.js production server, run the following command:
```
$ yarn start
```

To start the application in development mode, run the following command:
```
$ yarn dev
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

### Linting
`ESLint` is used as linting tool.

To run the lint use:
```
$ yarn lint
```

### Unit Tests
Unit tests are coded and run using `Jest`. (https://jestjs.io/ / https://testing-library.com/)

To run tests, run the following command:
```
$ yarn test
```

### Automation tests
Automation tests are coded and run using `Cypress`. (https://www.cypress.io/)

To run tests, run the following command:
```
$ yarn cy:run
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
