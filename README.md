# Auth0 Express API Sample

This repository contains a Node.js project that defines an Express API. You'll secure this API with Auth0 to practice making secure API calls from a client application.

## Get Started

Install the client project dependencies:

```bash
npm install
```

Create `.env` file under the project directory:

```bash
touch .env
```

Populate `.env` as follows:

```bash
API_PORT=7000
APP_ORIGIN=http://localhost:3000
AUTH0_AUDIENCE=
AUTH0_ISSUER=
```

Get values for `AUTH0_AUDIENCE` and `AUTH0_ISSUER` from your Auth0 Dashboard. You can find these values by following this path in the Dashboard:

**APIs > Your API > Quick Start > Node.js**

Locate the definition of `jwtCheck`. The object passed to `jwt` as an argument has an `audience` property, which is the value you need for `AUTH0_AUDIENCE`, and an `issuer`, which is the value you need for `AUTH0_ISSUER`.

Run the client project:

```bash
yarn start
```