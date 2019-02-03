# session of 2019-02
## overview

**Attendees:**

|name|status|email|phone
|---|---|---|---|
|Florian Chanal|RP|florian.chanal@redpelicans.com (fchanal@student.42.fr)|+33 7 51 67 34 92|
|Jean-Philippe Hoareau Méavilla|RP|jean-philippe.hoareau@redpelicans.com (jeahoare@gmail.com)|+33 6 20 62 65 48|
|Rabi Hrichi|?|eng.rabi.hr@gmail.com|+216 28 364 758|
|Hatem Bouhajja|?|hatembouhajja@gmail.com|-|
|Wael Azizi|?|wael.azizi@sesame.com.tn|-|

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

##schedule

**ideas (boite à idées):**
* D3JS charts with C3JS
* WP integration
* Final form with phone input, captcha and email (+confirmation)
* [css-grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

**day 1**
- [ ] [client introduction](https://docs.google.com/presentation/d/1nkelpLG-BikiiHWvfkUj7zxZDdMBx0pyCOhVnqDZLXE)
- [ ] [git introduction](http://nvie.com/posts/a-successful-git-branching-model/)
- [ ] [boilerplate introduction](https://github.com/facebook/create-react-app), [semver](https://semver.org/)
- [ ] setup boilerplate (single repository with a develop branch and a develop branch for each attendee)
- [ ] dummy pull request with feature branch (setup training git-flow and conventions)
- [ ] tictactoe presentation (UI)
- [ ] read [react documentation](https://reactjs.org/docs/hello-world.html) (quick start)
- [ ] read [react-elements-vs-react-components](https://medium.freecodecamp.org/react-elements-vs-react-components-fdc776705880)

**day 2**
- [ ] questions on day 1:
  - difference between `React.Element` and `React.Component`
  - difference between state and props
  - how to update the state?
- [ ] craft layout
- [ ] es6-import-export
  - [cheatsheet](https://hackernoon.com/import-export-default-require-commandjs-javascript-nodejs-es6-vs-cheatsheet-different-tutorial-example-5a321738b50f)
  - [value-import-export](http://es6-features.org/#ValueExportImport)
  - [default-and-wildcard](http://es6-features.org/#DefaultWildcard)
- [ ] [React.Fragment](https://reactjs.org/docs/fragments.html)
- [ ] react properties, rest parameter, react `PropTypes`
  - [typechecking-with-proptypes](https://reactjs.org/docs/typechecking-with-proptypes.html)
  - [rest-parameter](http://es6-features.org/#RestParameter)
- [ ] ways to style in react:
  - css stylesheets (webpack import, className attribute)
  - react style (style attribute, scoped, just JS)
  - [classnames](https://github.com/JedWatson/classnames)
  - [css-modules](https://github.com/css-modules/css-modules)
  - [MUI](https://material-ui.com/getting-started/usage/)
- [ ] [autoprefixer](https://github.com/postcss/autoprefixer)

**day 3**
- [ ] questions:
  - named export
  - wild as import
  - rest parameter
  - destructuring props
- [ ] [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [ ] conception of UI (declarative way, [mockup](https://docs.google.com/drawings/d/1Y5pBfaK2LEojsqKrj9JTdB8R-0HZk6AUcP6G-uXrf3Q/edit?usp=sharing))
- [ ] introduce composability (header with children)
- [ ] es6 function composition syntax

**day 4**
- [ ] dev?
- [ ] questions:
  - es6 string interpolation
  - flexbox wrapped centered layout
- [ ] pure function into class (React)
- [ ] read [react lifecycle](https://reactjs.org/docs/react-component.html#the-component-lifecycle)
- [ ] [es6-katas](http://es6katas.org/) (easy only: rest operator, destructuring, default parameters, modules, template strings)

**day 5**
- [ ] questions:
  - what is the purpose of the virtualDOM?
  - when React.Fragment is useful?
  - how to do a default export, how to import everything named export of a module (wild)?
  - what is the role of React?
- [ ] test environnement (package.json, jest, jest.config.js, coverage), travis
- [ ] test React components (shallow / mount, enzyme) and functions (sync, async, Error handling)
- [ ] introduce curry with the add() sample

