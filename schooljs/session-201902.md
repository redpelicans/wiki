# session of 2019-02

## overview

**Attendees:**

|name|status|email|phone
|---|---|---|---|
|Florian Chanal|RP|florian.chanal@redpelicans.com (fchanal@student.42.fr)|+33 7 51 67 34 92|
|Jean-Philippe Hoareau Méavilla|RP|jean-philippe.hoareau@redpelicans.com (jeahoare@gmail.com)|+33 6 20 62 65 48|
|Rabi Hrichi|?|eng.rabi.hr@gmail.com|+216 28 364 758|
|Wael Azizi|give up day 2|wael.azizi@sesame.com.tn|-|

**Todo:**
- [x] create google accounts (for RP attendees)
- [x] invite to schoolJS slack chan

**General information:**
* start on the 4th of February 2019
* normal day schedule: conf calls 9h30 and 14h30 on hangout

**Soft pre-requisites:**
* internet connection good enough for video calls
* webcam and headset
* quiet place where it's possible to talk

**Technical pre-requisites:**
* ideally a unix OS
* nodejs and git
* an editor (atom, vim, sublime text, vscode)
* a browser (chrome, firefox)

> run `node --version` and `git --version` in the console

## schedule

**Todo (boite à idées):**
* D3JS charts with C3JS
* WP integration
* Final form with phone input, captcha and email (+confirmation)
* [css-grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
* final form with phone input
* react context with user, display current user in the app (header)

### week1

**day 1**
- [x] [client introduction](https://docs.google.com/presentation/d/1R48RLleag1PTSy4-CzMdhlr02yTUp2JTGXdstxGfFMU/edit#slide=id.g145b507c17_0_109)
- [x] [git introduction](http://nvie.com/posts/a-successful-git-branching-model/)
- [x] [boilerplate introduction](https://github.com/facebook/create-react-app), [semver](https://semver.org/)
- [x] setup boilerplate (single repository with a develop branch and a develop branch for each attendee)
- [x] dummy pull request with feature branch (setup training git-flow and conventions)
- [x] tictactoe presentation (UI)
- [x] read [react documentation](https://reactjs.org/docs/hello-world.html) (quick start)
- [x] read [react-elements-vs-react-components](https://medium.freecodecamp.org/react-elements-vs-react-components-fdc776705880)

**day 2**
- [x] questions on day 1:
  - difference between `React.Element` and `React.Component`
  - how to fix a bug in production (git)
  - Can we modify props?
- [x] [autoprefixer](https://github.com/postcss/autoprefixer), [show webpack diagram](https://docs.google.com/presentation/d/1R48RLleag1PTSy4-CzMdhlr02yTUp2JTGXdstxGfFMU/edit#slide=id.g145b507c17_0_109)
- [x] es6-import-export
  - [cheatsheet](https://hackernoon.com/import-export-default-require-commandjs-javascript-nodejs-es6-vs-cheatsheet-different-tutorial-example-5a321738b50f)
  - [value-import-export](http://es6-features.org/#ValueExportImport)
  - [default-and-wildcard](http://es6-features.org/#DefaultWildcard)
- [x] react properties, rest parameter, react `PropTypes`
  - [typechecking-with-proptypes](https://reactjs.org/docs/typechecking-with-proptypes.html)
  - [rest-parameter](http://es6-features.org/#RestParameter)
  - [spread-operator](http://es6-features.org/#SpreadOperator)
  - [destructuring](http://es6-features.org/#ParameterContextMatching)
- [x] [katas](http://es6katas.org/) (modules, spread, rest, destructuring)
- [x] ways to style in react:
  - css stylesheets (webpack import, className attribute)
  - react style (style attribute, scoped, just JS)
  - [classnames](https://github.com/JedWatson/classnames)
  - [css-modules](https://github.com/css-modules/css-modules)
  - [MUI](https://material-ui.com/getting-started/usage/)
- [ ] craft history (stateless, no props)

**day 3**

- [x] [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [x] conception of UI (declarative way)
- [x] craft cards

**day 4**
- [x] Add MUI in project
- [x] explainWebpackDevServer, bundle.js, css , how App is launched
- [x] craft cards with MUI

**day 5**
- [x] introduce composability (header with children)

### week2

**day 6**
- [ ] code review (header, layout with MUI and Grid)
- [ ] test environnement (package.json, jest, jest.config.js, coverage), travis
- [ ] test React components (shallow / mount, enzyme) and functions (sync, async, Error handling)
- [ ] readings FP for day 7:
  - [ ] read [what-is-functional-programming](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
  - [ ] read [thinking-in-ramda](http://randycoulman.com/blog/categories/thinking-in-ramda/)
  - [ ] read [introducing-ramda](http://buzzdecafe.github.io/code/2014/05/16/introducing-ramda)
  - [ ] read [why-ramda](http://fr.umio.us/why-ramda/)
  - [ ] watch [undercore-is-doing-wrong](https://www.youtube.com/watch?v=m3svKOdZijA&app=desktop)

**day 7**
- [ ] tutorial + exercices (https://bitbucket.org/redpelicans/fptraining) with [ramda](http://ramdajs.com/)
- [ ] history in state and craft history+chart (c3.js), all tested

**day 8**
- [x] craft chart, board, history

**day 9**
- [x] board from state (step6)

**day 10**
- [x] board from state (step6)

### week3

**day 11**
- [ ] login form with controlled/uncontrolled in MUI ([Form](https://material-ui.com/getting-started/page-layout-examples/sign-in/)) `tictactoe_2018:step7`
- [ ] auth hoc `tictactoe_2018:step7-hoc`
- [ ] withMouse & withLog hocs (exercises)

**day 12**
- [ ] refactor login form with final form `tictactoe_2018:step7-final-form`
- [ ] tutorial + exercices (https://bitbucket.org/redpelicans/fptraining) with [ramda](http://ramdajs.com/)

**day 13**
- [x] ramda exercises to check
- [x] recompose on App + withAuth

**day 14**
- [x] recompose
- [x] wip on game

**day 15**
- [x] 100% test coverage game.js
- [x] 100% testcomponent snapshot
- [x] test enhance + enhance(Component)
- [x] wip full game playable
- [x] mockey patching

### week4

**day 16**
- [x] Promises
  - [x] read [what-is-a-promise](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-a-promise-27fc71e77261)
  - [x] read [the-promise-of-a-burger-party](https://kosamari.com/notes/the-promise-of-a-burger-party)
  - [x] do [promise-it-wont-hurt](https://github.com/stevekane/promise-it-wont-hurt)
- [ ] simulateClick
- [ ] jest.fn

**day 17**
- [ ] Promises : stream of icons instead of sdtatic incon in HeaderLeft
- [ ] Promises : 10 fruits per cell
- [ ] Promises : fruits until plane
- [ ] pragmatic introduction to fetch to prepare MARVEL
- [ ] componentDidMount flow fetch
- [ ] MARVEL instructions
- [ ] withAuth

**day 18**
- [ ] MARVEL

**day 19**
- [x] Marvel correction
- [x] Redux Starting guide

**day 20**
- [x] Marvel with one state
- [x] https://egghead.io/courses/getting-started-with-redux

**day 21**
- [x] Marvel with redux
- [x] Tictactoe with Redux

**day 22**
- [x] Tictactoe with Redux

**day 23**
- [x] Tictactoe with Redux
- [x] Tictactoe with thunk
- [x] Tictactoe with server side requests


**day 24**
- [x] test reducer
- [x] build own middleware
- [x] build test middleware

**day25**
- [x] test all

**day26**
- [x] review tests
- [x] introduce jest.mock() to tests async actions

**day27**
- [x] reselect
- [x] rendering optimizations

**day28**
- [x] promises workshop

**day29**
- [x] optimize rendering:
  - virtual DOM, diffing algo, explicit mutations
  - Component, PureComponent, shouldComponentUpdate
  - react devtools highlights, console.log in renders
  - exercise: https://lucybain.com/blog/2018/react-js-pure-component/
  - redux#connect, recompose#shouldUpdate, recompose#pure

**day30**
- [x] update tictactoe

**day31**
- [ ] routes

**day32**
- [x] fruits server

**day33**
- [x] marvel

**day34**
- [ ] tests fruits
- [ ] tests mongodb-gcs-backup




