# Boilerplate: ES Modules, Stage 2, Webpack, React.

Boilerplate for **React Webapps** that use **ES Modules** and stage2 **Class Properties**.


## NPM Scripts

The following commands are available:
 - **npm install**: Install dependencies
 - **npm start**: Starts the Webpack Dev Server
 - **npm run build**: Generate production bundles of `/src/entry.js` to `/www` folder
 - **npm run analyze**: Generates production bundles, and opens Webpack Bundle Analyzer
 - **npm test**: Eslints the `/src` folder, runs Mocha unit tests in Karma, and runs Code Coverage (in Karma too)


## Visual Studio Code

Once you have Webpack Dev Server running (using `npm start`), open the VSCode debugger.
It is already setup to open http://localhost:8000, so you get both *remote debugging* and *livereload*.

Also, despite everything is merely ES2015 Javascript, it has Flow-like **linting and Intellisense**
using VSCode's built-in *Typescript* integration (see `/tsconfig.json` to customize its settings).
and *Eslint* (listed in the workspace recommended extensions).


## Test and Analyze

Unit tests use **Mocha**, **Enzyme** and **Sinon**, and are run in **Karma**.
You can change the list of webdrivers in `/karma.conf.js` (currently: IE, Chrome, and Firefox).
Results are outputted in `/logs/karma.tests.html`.

**Code Coverage** also runs in Karma, and is outputted in `/logs/coverage`.

**Webpack Bundle Analyzer** generates `/www/webpack.stats.html` and `/www/webpack.stats.json`.

