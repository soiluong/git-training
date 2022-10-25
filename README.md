yenting changes 123

Client repo for Sprout frontend

- [Project setup & develop](#project-setup--develop)
- [Code formatting](#code-formatting)
- [Testing](#testing)
- [Supported browsers](#supported-browsers)
- [Codebase overview](#codebase-overview)

## YentingLay

Main branch is automatically deployed to the dev environment
To deploy code to a client environment (includes prod and nonprod) create a gitlab tag from the UI from the main branch or any commit on it using the commit reference.
At any time any tag or branch can be deployed to any environment using the git pipelines to do a deploy. https://gitlab.com/sprout-ai/foundation-product/frontend-web/-/pipelines/new

editing check

### Setup

Clone the repo, run setup and

edit

```shell
git clone <ssh-link>

cp .env.example .env

npm run setup

npm run dev
```

#### To disable Mock Service Worker

```dotenv
# ensure this environment variable is set to false in your .env file
VITE_MSW=false
```

## Code formatting

Ensure you have configured your chosen IDE to use Prettier on save and to use the rules that it will automatically
pick up from `package.json`.

## Testing

Ensure you have already installed the dependencies as instructed above.

### Linting

Running ESLint:

```shell
npm run lint
```

### Static test

Running TSC:

```shell
npm run typecheck
```

### Unit tests

Running Vitest:

```shell
npm run test
```

### E2E tests

To run testing in development:

1. Ensure you have the client running first as instructed above.
2. Your `.env` file should have the environment variables `VITE_RUNNING_E2E=true` `OKTA_USERNAME` `OKTA_PASSWORD` and `VITE_OKTA_DOMAIN` setup correctly
3. Open Cypress in a separate terminal: `npm run cy:open`
4. Select your chosen browser in Cypress App
5. Click on `Run # integration specs`

OR

Run the above steps in one command: `npm run test:e2e:dev`

OR

Build the client first then run the client and Cypress together:

```shell
npm run test:e2e:run
```

## Codebase overview

This project was originally bootstrapped with [Create React App](https://github.com/facebook/create-react-app).
Now migrated to [Vite](https://vitejs.dev/)

TODO: add more explanation of the repo, dependencies and structure here

## Translations

https://docs.google.com/spreadsheets/d/1AdRwFZLZRPSfcaSG6f4OHy8ckVUHHgfVUUd8hJR1ask

editing

## Troubleshooting

```shell
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --ignore-certificate-errors --unsafely-treat-insecure-origin-as-secure=https://local.sprout.ai:8080
```

My new changes here
hello
hello^)
hi
