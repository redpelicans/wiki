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
* tests async, middleware
* react-router

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

**day 11**
- [ ] login form with controlled/uncontrolled in MUI ([Form](https://material-ui.com/getting-started/page-layout-examples/sign-in/)) `tictactoe_2018:step7`
- [ ] auth hoc, display current user in the app (header) `tictactoe_2018:step7-hoc`
- [ ] refactor login form with final form `tictactoe_2018:step7-final-form`

**day 12**
- [ ] withMouse hoc
- [ ] final form with phone input
- [ ] react context with user

**day 13**
- [ ] _we want to play_: review workflow, make board playable

**day 14**
- [ ] _we want to play_: review workflow, make board playable

**day 15**
- [ ] _we want to play_: review workflow, make board playable

**day 16**
- [ ] pragmatic introduction to fetch to prepare MARVEL
- [ ] componentDidMount flow fetch
- [ ] ?

**day 17**
- [ ] ?
- [ ] MARVEL instructions

**day 18**
- [ ] MARVEL

**day 19**
- [ ] Flux, reducer (sfs like)

**day 20**
- [ ] ?
