# Sprout - Frontend Web

Client repo for Sprout frontend

- [Project setup & develop](#project-setup--develop)
- [Code formatting](#code-formatting)
- [Testing](#testing)
- [Supported browsers](#supported-browsers)
- [Codebase overview](#codebase-overview)

## git push --set-upstream

## Releases to client environments
Main branch is automatically deployed to the dev environment
To deploy code to a client environment (includes prod and nonprod) create a gitlab tag from the UI from the main branch or any commit on it using the commit reference.
At any time any tag or branch can be deployed to any environment using the git pipelines to do a deploy. https://gitlab.com/sprout-ai/foundation-product/frontend-web/-/pipelines/new

## Project setup & develop

### System requirements

- Node.js >=16.0.0 LTS
- NPM >=8.0.0

### Setup

Clone the repo, run setup and start development:

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
````

### Static test

Running TSC:

```shell
npm run typecheck
````
