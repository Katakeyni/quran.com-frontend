## Quran.com
This is the project soon to be the Quran.com facing site. This is built in
Reactjs + Flux (Fluxible by Yahoo) + Expressjs + Webpack. It is isomorphic (javascript shared
between both the server and the client) for SEO reasons.

#### Getting started
Simply clone this repo, then run `npm install` to install all the required node_modules.
From there, you are ready to go!

#### Developing
To start the app, run `npm run dev` which will
run both the server and the client (webpack) to compile upon edits. Go to localhost:8001 in your browser, not 8000 (that is just the express server).

#### Tests
Run `npm run test:watch` to run the tests locally and watching. Otherwise use `npm run test` for CI level tests.

We also have nightwatch function tests. You can install nightwatch globally and can run tests like this:
```
nightwatch --test tests/functional/specs/Index_spec.js
```

#### Backend
Current at: https://github.com/quran/quran-api-rails
DB is private, message me for acceess.

#### How to contribute
Fork this repo, then create a PR for specific fixes, improvements, etc. We trust that
you will not steal this, this is at the end of the day for the sake of Allah and we
all have good intentions while working with this project. But I must stress, stealing
this is unacceptable.

#### Design
We currently use InvisionApp. Again, contact me if you'd like access to it.

#### Making sure main.js is small
Follow: https://www.npmjs.com/package/webpack-bundle-size-analyzer
```
env NODE_ENV=development webpack --json > bundle-stats.json
subl bundle-stats.json #so that you can the output
analyze-bundle-size bundle-stats.json
```
