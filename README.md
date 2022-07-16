# Coding Challenge Backend

Your challenge is to create a Node.js server to serve as the (backend) API for [the frontend](https://github.com/davidhartsough/coding-challenge-frontend) part of this coding challenge.

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
3. [Submission](#submission)

### Installation

Do NOT fork this repo.

1. Clone this repo (and `cd` into it)
2. Install the dependencies using [yarn](https://classic.yarnpkg.com/lang/en/) or npm. (I used yarn [hence the `yarn.lock` file].)

### Implementation

(in any order you prefer)

- In `src/server.ts`, follow the instructions on lines 24-28 and 30.
- In `src/get-metadata.ts`, follow the instructions on lines 12-18 and 23.

For help, use the Jest tests in `src/get-metadata.test.ts`.

### Submission

Once again, do NOT fork this repo.

When you're done and ready to submit your code in the application, follow these steps to push your code to your own GitHub repo:

1. Create a new repository on GitHub.
2. Remove the remote origin with: `git remote rm origin`
3. Add the remote origin of your new repo with: `git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git`
4. Push your code to your new repo with: `git push -u origin master` (or `main` or whatever your preferred branch name is)
5. Copy the URL to your repo and add it to the application (https://github.com/YOUR-USERNAME/YOUR-REPO-NAME). (If you wish to keep your new repo private, you must add me, `davidhartsough`, as a collaborator: https://github.com/YOUR-USERNAME/YOUR-REPO-NAME/settings/access)

## Scripts

In the root project directory, you can run:

### `yarn start`

Runs the server at [http://localhost:5000](http://localhost:5000)

### `yarn test`

Runs the Jest tests.

## Language

- [Node.js](https://nodejs.dev/learn)
- [TypeScript](https://www.typescriptlang.org/docs/)

## Linting/Formatting

- [ESLint](https://eslint.org/) - linting
- [Prettier](https://prettier.io/) - formatting

As you complete the challenge, you are encouraged to lint and format your code.

In the root project directory, you can run the following scripts:

```bash
yarn lint
```

Or, to let eslint try to fix your code according to the linter and formatter standards, run:

```bash
yarn lint:fix
```
