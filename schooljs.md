<!-- TITLE: Schooljs -->
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
> flexbox, cssgrid, composability of react components

- [ ] dev2 update dev1 with props, `PropTypes` and data from a store
- [ ] dev3 style dev2 with blueprintjs and glamorous
- [ ] [es6-string-interpolation](http://es6-features.org/#StringInterpolation)
- [ ] questions on day 2 readings:
  - named export
  - wild as import
  - rest parameter
  - destructuring props
- [ ] [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [ ] [css-grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [ ] conception of UI (declarative way)
- [ ] dev4 implement missions page (layout)
- [ ] introduce composability (header with children, generic card for mission)

**day 4:**
> es6, react lifecycle

- [ ] read [es6 introduction](https://ponyfoo.com/articles/es6)
- [ ] read [react lifecycle](https://reactjs.org/docs/react-component.html#the-component-lifecycle)
- [ ] dev5 play with react lifecycle ([timer](https://reactjs.org/docs/state-and-lifecycle.html))

**day 5 (wednesday 10/1):**
> UI tests with Eric (jest, snapshots, travis, coverage)

**day 6:**
> flux

- [ ] read [flux introduction](https://facebook.github.io/flux/docs/in-depth-overview.html#content)
- [ ] conception of flows (flow scheme)
- [ ] es6 function composition syntax
- [ ] dev6 flux implementation (with delete mission)

**day 7:**
> HOC, react context, conception (smart vs dumb components, ui data in state)

- [ ] read [smart-vs-dumb-components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0)
- [ ] introduce HOC
- [ ] introduce React context
- [ ] dev7 refine dev6 with HOC and context
- [ ] dev8 use state for UI data (hover on mission to show actions)

**day 8:**
> redux

- [ ] [redux training](https://egghead.io/courses/getting-started-with-redux)
- [ ] dev9 redux migration

**day 9 (oecd call for tender 3pm):**
> reselect

- [ ] introduce [reselect](https://github.com/reactjs/reselect)
- [ ] dev10 implement spotlight and sorts
- [ ] watch [event loop](https://www.youtube.com/watch?v=8aGhZQkoFbQ)

**day 10 (wednesday 17/1):**
> Unit tests with Eric (reducers, actions, selectors)

**day 11:**
> FP

- [ ] read [what-is-functional-programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
- [ ] read [thinking-in-ramda](http://randycoulman.com/blog/categories/thinking-in-ramda/)
- [ ] dev11 rewrite selectors with [ramda](http://ramdajs.com/)
- [ ] introduce curry with the add() sample

**day 12:**
> FP, promise

- [ ] FP test with https://bitbucket.org/redpelicans/fptraining
- [ ] read [the-promise-of-a-burger-party](https://kosamari.com/notes/the-promise-of-a-burger-party)
- [ ] do [promise-it-wont-hurt](https://github.com/stevekane/promise-it-wont-hurt)

**day 13:**
> Promise

- [ ] test onearmedbandit

**day 14:**
> client/server, fetch, redux-thunk

- [ ] introduction to client/server, http verbs, restful
- [ ] read [fetch API](https://davidwalsh.name/fetch)
- [ ] dev11 use redux-thunk to fetch missions and delete a mission (fetching, success, error)

**day 15 (wednesday 24/1):**
> async tests with Eric

**day 16:**
> redux midleware

- [ ] [redux middleware](https://redux.js.org/docs/advanced/Middleware.html)
- [ ] dev12 implement a middleware to block blacklisted actions

**day 17:**
add mission and forms

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