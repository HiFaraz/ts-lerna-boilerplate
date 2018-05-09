# ts-lerna-boilerplate
Boilerplate for Typescript packages in a Lerna monorepo

## Quick start

1. Clone this repo using `git clone --depth=1 https://github.com/HiFaraz/ts-lerna-boilerplate.git`
2. Move to the appropriate directory: `cd ts-lerna-boilerplate.`
3. Run `npm run setup` in order to install dependencies and clean the git repo.

## Compiling Typescript code

Typescript code for each package must live in the `src` folder and will be emitted to the `lib` folder. Run `npm run compile` to compile.

To clean compiled code run `npm run clean`

## Lint

Run `npm run lint` to run TSLint. To run with the auto-fix mode, run `npm run lint -- --fix`

## Tests

Tests are run with the Jest framework. To run tests on all packages, run `npm test`.

## CI build pipeline

`npm run build` is a composite command which runs:

1. `npm run lint`
2. `npm run clean`
3. `npm run build`