<!-- TITLE: session2018-01 -->
<!-- SUBTITLE: All about training sessions -->

# session of 2018-01
## overview

**Attendees:**
* Thomas Tridon (RP) - thomas.tridon@redpelicans.com - ttridon@gmail.com
* Mike Velluet (RP) - mike.velluet@redpelicans.com - mike.velluet@gmail.com
* Arnaud Le Floch (RP) - arnaud.lefloch@redpelicans.com - a.lefloch2491@gmail.com
* Mahmoud chebbou - mahmoud.chebbou@nearteam.fr

> [ ] create google accounts for RP attendees
> [ ] invite to schoolJS slack chan

**General information:**
* start on the 4th of January 2018
* normal day schedule: conf calls 9h30 and 14h30 on hangout

**Soft pre-requisites:**
* internet connection good enough for video calls
* webcam and headset
* quiet place where it's possible to talk

**Technical pre-requisites:**
* ideally a unix OS, if windows then install [babun](http://babun.github.io/) to have a proper shell
* nodejs and git
* an editor (atom, vim, sublime text, vscode)
* a browser (chrome, firefox)

> run `node --version` and `git --version` in the console

## schedule

**unplanned concept/tasks and dropped (uncheck) tasks:**
- async/await
- react-router
- avatar component (oneplus is nice)
- login feature
- media-query
- react-motion and FAC
- [ ] dev play with react lifecycle ([clock](https://openclassrooms.com/courses/build-web-apps-with-reactjs/build-a-ticking-clock-component), use props hooks only)

**day 1 (4/1):**
> client, git, boilerplate, react, components vs elements

- [x] [client introduction](https://docs.google.com/presentation/d/1nkelpLG-BikiiHWvfkUj7zxZDdMBx0pyCOhVnqDZLXE)
- [x] [git introduction](http://nvie.com/posts/a-successful-git-branching-model/)
- [x] [boilerplate introduction](https://github.com/redpelicans/mission-impossible), [semver](https://semver.org/)
- [x] setup boilerplate (single repository with a dev branch for each attendee)
- [x] read [react documentation](https://reactjs.org/docs/hello-world.html) (quick start)
- [x] read [react-elements-vs-react-components](https://medium.freecodecamp.org/react-elements-vs-react-components-fdc776705880)

**day 2:**
> props, proptypes, styling

- [x] questions on day 1 readings:
  - difference between `React.Element` and `React.Component`
  - difference between state and props
  - how to update the state?
- [x] [dev1](https://github.com/redpelicans/mission-impossible/commit/8d32357eba786f3ad9042180d24c3976e0e77570) list of missions (stateless, no props)
- [x] es6-import-export
  - [cheatsheet](https://hackernoon.com/import-export-default-require-commandjs-javascript-nodejs-es6-vs-cheatsheet-different-tutorial-example-5a321738b50f)
  - [value-import-export](http://es6-features.org/#ValueExportImport)
  - [default-and-wildcard](http://es6-features.org/#DefaultWildcard)
- [x] [React.Fragment](https://reactjs.org/docs/fragments.html)
- [x] react properties, rest parameter, react `PropTypes`
  - [typechecking-with-proptypes](https://reactjs.org/docs/typechecking-with-proptypes.html)
  - [rest-parameter](http://es6-features.org/#RestParameter)
- [ ] ~~dev2 update dev1 with props, `PropTypes` and data from a store~~
- [x] ways to style in react:
  - css stylesheets (webpack import, className attribute)
  - react style (style attribute, scoped, just JS)
  - [classnames](https://github.com/JedWatson/classnames)
  - [css-modules](https://github.com/css-modules/css-modules)
  - [glamorous](https://github.com/paypal/glamorous)
  - [blueprintjs](http://blueprintjs.com/docs/)
- [x] [autoprefixer](https://github.com/postcss/autoprefixer)
- [ ] ~~dev3 style dev2 with blueprintjs and glamorous~~

**day 3:**
> flexbox, composability of react components

- [x] dev2 update dev1 with props, `PropTypes` and data from a store
- [ ] ~~dev3 style dev2 with blueprintjs and glamorous~~
- [x] [es6-string-interpolation](http://es6-features.org/#StringInterpolation)
- [x] questions on day 2 readings:
  - named export
  - wild as import
  - rest parameter
  - destructuring props
- [x] [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [x] [css-grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [x] conception of UI (declarative way, [mockup](https://docs.google.com/drawings/d/1Y5pBfaK2LEojsqKrj9JTdB8R-0HZk6AUcP6G-uXrf3Q/edit?usp=sharing))
- [x] introduce composability (header with children, generic card for mission)
- [x] es6 function composition syntax
- [ ] ~~dev4 implement missions page (layout and composed header)~~

**day 4:**
> es6, react lifecycle

- [x] [dev3](https://github.com/redpelicans/mission-impossible/commit/6176192c17b66455059b4c00a5f60f25b77371f9) style dev2 with blueprintjs and glamorous
- [x] [dev4](https://github.com/redpelicans/mission-impossible/commit/336e2eb3296ad8f52d23c1364c96617f747e93a8) implement missions page (layout and composed header)
- [x] questions:
  - es6 string interpolation
  - flexbox wrapped centered layout
- [x] pure function into class (React)
- [x] read [react lifecycle](https://reactjs.org/docs/react-component.html#the-component-lifecycle)
- [x] [es6-katas](http://es6katas.org/) (easy only: rest operator, destructuring, default parameters, modules, template strings)

**day 5 (wednesday 10/1):**
> es6, react lifecycle, UI tests (jest, snapshots, travis, coverage?)

- [x] test environnement (package.json, jest, jest.config.js, coverage), travis
- [x] [dev5](https://github.com/redpelicans/mission-impossible/commit/9eac8c3634c35b3189a404c72b5754e265c60926) test React components (shallow / mount, enzyme) and functions (sync, async, Error handling)
- [x] introduce curry with the add() sample
- [x] questions:
  - @arnaud: what is the purpose of the virtualDOM?
  - @thomas: when React.Fragment is useful?
  - @mahmoud: how to do a default export, how to import everything named export of a module (wild)?
  - @mike: what is the role of React?

**day 6:**
> flux

- [x] read [flux introduction](https://facebook.github.io/flux/docs/in-depth-overview.html#content)
- [x] conception of flows (flow scheme)
- [ ] ~~dev6 flux implementation (peer programming with delete mission, toggle mission, delete selected missions)~~

**day 7:**
> HOC

- [x] questions:
  - what is MVC?
  - explain the flux flow?
  - what are the key elements of flux?
  - most important prop of a reducer?
  - what is immutability?
- [x] [dev6](https://github.com/redpelicans/mission-impossible/commit/7a9f9119f6369145cd3a27bca70d6aa98a17c4df) flux implementation (peer programming with delete mission, toggle mission, delete selected missions)
- [x] introduce HOC
- [x] read [higher-order-components](https://reactjs.org/docs/higher-order-components.html)
- [ ] ~~dev7 refine dev6 with Connect HOC, Logger HOC, Glamour HOC~~

**day 8:**
> React context, React state for UI

- [x] questions:
  - why writing tests? (catch bugs before they happen, executable documentation, save time, push to write better code)
  - nature of a HOC, some usecases?
- [x] [dev7](https://github.com/redpelicans/mission-impossible/commit/a1715c4a78c283f5d49b9b94376494ed8b92b669) refine dev6 with Connect HOC, Logger HOC, Glamour HOC
- [x] read [react-context](https://reactjs.org/docs/context.html)
- [x] dev8 refine dev7 with context
- [x] read [react-events](https://reactjs.org/docs/events.html) and [handling-events](https://reactjs.org/docs/handling-events.html)
- [x] dev9 use state for UI data (hover on mission to show actions)

**day 9 (oecd call for tender 3pm):**
> redux and middleware

- [x] questions:
  - what is the role of the Provider?
  - what is the role of connect?
  - what is the store?
  - what is encapsulation?
- [x] [dev10](https://github.com/redpelicans/mission-impossible/commit/4c80a35edaf279d2e1f4a1b0cbb87cc77a601e02) redux migration
- [] ~~[dev11](https://github.com/redpelicans/mission-impossible/commit/5b589455e60d19a9a29081254872317bb86d7a95) implement 2 middlewares (logger and firewall) and put them in action~~
- [x] [redux middleware](https://redux.js.org/docs/advanced/Middleware.html)
- [x] read [smart-vs-dumb-components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0)
- [x] [redux training](https://egghead.io/courses/getting-started-with-redux)

**day 10 (wednesday 17/1):**
> FP

- [ ] read [what-is-functional-programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
- [ ] read [thinking-in-ramda](http://randycoulman.com/blog/categories/thinking-in-ramda/)
- [x] read [introducing-ramda](http://buzzdecafe.github.io/code/2014/05/16/introducing-ramda)
- [x] read [why-ramda](http://fr.umio.us/why-ramda/)
- [x] watch [undercore-is-doing-wrong](https://www.youtube.com/watch?v=m3svKOdZijA&app=desktop)
- [x] tutorial + exercices (https://bitbucket.org/redpelicans/fptraining) with [ramda](http://ramdajs.com/)

**day 11:**
> reselect

- [x] questions:
  - what is ramda?
  - what is a pure function?
- [x] [dev11](https://github.com/redpelicans/mission-impossible/commit/5b589455e60d19a9a29081254872317bb86d7a95) implement 2 middlewares (logger and firewall) and put them in action + middleware test
- [ ] introduce [reselect](https://github.com/reactjs/reselect)
- [ ] dev inject relationshios (people and companies) in missions and implement spotlight and sorts
- [ ] read [computing-derivated-data](https://redux.js.org/docs/recipes/ComputingDerivedData.html)

**day 12:**
> promise

- [ ] questions:
	- what is a pure function?
	- what is currying and partial?
- [ ] read [the-promise-of-a-burger-party](https://kosamari.com/notes/the-promise-of-a-burger-party)
- [ ] do [promise-it-wont-hurt](https://github.com/stevekane/promise-it-wont-hurt)

**day 13:**
> Promise

- [ ] test onearmedbandit

**day 14:**
> client/server, fetch, redux-thunk

- [ ] introduction to client/server, http verbs, restful
- [ ] read [fetch API](https://davidwalsh.name/fetch)
- [ ] dev use redux-thunk to fetch missions and delete a mission (fetching, success, error)

**day 15 (wednesday 24/1):**
> async tests with Eric

**day 16:**
> ?

- [ ] read [es6 introduction](https://ponyfoo.com/articles/es6)
- [ ] watch [event loop](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

**day 17:**
- [ ] add mission and forms
- [ ] [css-grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

**day 18:**
add mission and forms

**day 19:**
> optimize rendering

- [ ] React#shouldComponentUpdate()
- [ ] React.PureComponent
- [ ] react-redux#connect() with option: { pure: true } (default)
- [ ] reselect
- [ ] recompose

**day 20 (wednesday 31/1):**
> FAC

- [ ] read [FAC introduction](https://cdb.reacttraining.com/use-a-render-prop-50de598f11ce)
- [ ] do https://github.com/eric-basley/hocAndCo (branches vanilla, hoc, child, cat, motion)

**day 21:**
- [ ] test marvel

**day 22 (friday 2/2):**
wrap up