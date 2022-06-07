# Coding Challenge Backend

Your challenge is to create a Node.js server to serve as the (backend) API for the frontend part of this coding challenge.

In the end, you'll be able to send a POST request to this server with a JSON payload containing a URL and it will return important and relevant metadata from the site at the given URL, including the site name, title, description, keywords, and author.

Example:

```bash
# request
curl -X POST \
  -H "Content-Type: application/json" \
  -d '{"url":"https://davidhartsough.com/"}' \
  http://localhost:5000/
# result
{"url":"https://davidhartsough.com","siteName":"David Hartsough","title":"David Hartsough","description":"David Hartsough is widely regarded as a happy human, drummer, developer, designer, wannabe psychologist/philosopher, and stuntman — more or less.","keywords":"david,hartsough,davidhartsough,human,drummer,developer,designer,psychologist,philosopher,stuntman","author":"David Hartsough"}
```

## Steps

1. [Installation](#installation)
2. [Implementation](#implementation)

## Installation

1. Clone this repo (and `cd` into it)
2. [Install `yarn`](https://classic.yarnpkg.com/en/docs/install)
3. Run `yarn`

### Linting/Formatting

- [ESLint](https://eslint.org/) - linting JS
- [Prettier](https://prettier.io/) - formatting JS and CSS

## Implementation

(in any order you prefer)

- In `src/server.ts`, follow the instructions on lines 24-28 and 30.
- In `src/get-metadata.ts`, follow the instructions on lines 12-18 and 23.

For help, use the Jest tests in `src/get-metadata.test.ts`.

## Available Scripts

In the root project directory, you can run:

### `yarn start`

Runs the server at [http://localhost:5000](http://localhost:5000)

### `yarn test`

Runs the Jest tests.
