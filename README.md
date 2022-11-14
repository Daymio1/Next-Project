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


#### **_Husky_**
Husky is used to lint the commit messages, run tests, lint code when you commit or push.

Documentation: https://typicode.github.io/husky/#/

#### **_I18Next_**
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

To open Cypress, run the following command:
```
$ yarn cy
```

To run tests, run the application then run the following command:
```
$ yarn cy:run
```

To run the application and the test runner in **CI** (headless), run the following command:
```
$ yarn e2e:ci
```

_CI refers to "Continous Integration" and is just referring to a build pipeline._

#### Details about the env variables required to run tests (without the exact values) read the documentation: https://docs.cypress.io/guides/guides/environment-variables#Option-1-configuration-file

- Example of .env variables:
```JavaScript
export default defineConfig({
  env: {
    auth0_username: process.env.AUTH0_USERNAME,
    auth0_password: process.env.AUTH0_PASSWORD,
    auth0_issuer_base_url: process.env.AUTH0_ISSUER_BASE_URL,
  },
});
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

To build the Docker image, run the following command:
```
$ docker build <path-to-dockerfile>
```

- .env variables required to build the docker image:
```Dockerfile
ARG AUTH0_SECRET
ARG AUTH0_BASE_URL
ARG AUTH0_ISSUER_BASE_URL
ARG AUTH0_CLIENT_ID
ARG AUTH0_CLIENT_SECRET
```
