# SpaHarryPother

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 19.1.6.

A Single Page Application (SPA) built with Angular 19 that fetches and displays Harry Potter universe data (characters and spells) using the public Harry Potter API.

## Tech Stack

- **Framework**: Angular 19.1 (Standalone components)
- **Language**: TypeScript 5.7
- **HTTP Client**: Angular `HttpClient` (`provideHttpClient`)
- **Reactive Programming**: RxJS 7.8
- **Testing**: Jasmine 5.5 & Karma 6.4

## Prerequisites

- [Node.js](https://nodejs.org/) (compatible with Angular 19)
- [npm](https://www.npmjs.com/) (bundled with Node.js)
- [Angular CLI](https://angular.dev/tools/cli) (optional for global commands, `npm install -g @angular/cli`)

## Installation

Clone the repository and install dependencies:

```bash
npm install
```

## Available Scripts

In the project directory, you can run:

- `npm start` (or `ng serve`): Starts the development server at `http://localhost:4200/`.
- `npm run build` (or `ng build`): Compiles the application into the `dist/spa-harry-pother` folder.
- `npm run watch`: Builds the project in development mode with watch mode enabled.
- `npm test` (or `ng test`): Runs unit tests with Karma.

## Development server

To start a local development server, run:

```bash
ng serve
```

(or `npm start`)

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

(or `npm test`)

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Project Structure

```text
src/
├── app/
│   ├── app.component.{ts,html,css,spec.ts}   # Root component fetching characters
│   ├── app.config.ts                         # Application config & providers (HttpClient, Router)
│   ├── app.routes.ts                         # Routing configuration
│   ├── character.ts                          # Character and Wand interfaces
│   ├── spell.ts                              # Spell interface
│   └── spells/
│       └── spells-list/                      # Component fetching and displaying spells
│           ├── spells-list.component.{ts,html,css,spec.ts}
├── index.html                                # Main HTML file
├── main.ts                                   # Application bootstrap entry point
└── styles.css                                # Global application styles
```

## External APIs

The application integrates with the following public endpoints:

- `GET https://hp-api.onrender.com/api/characters`: Retrieves the list of Harry Potter characters (name, image, attributes).
- `GET https://hp-api.onrender.com/api/spells`: Retrieves the list of spells (name, description).

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.

