# session of 2019-09

**todo:**
- service workers
- hoc, render as prop, fac
- tricky questions in interviews
- atelier wp landing page koopt (use rabi)

setup copy of tictactoe:
```
git clone https://gitlab.com/redpelicans/tictactoe-winter-2019.git
cd tictactoe-winter-2019
git remote set-url origin https://gitlab.com/redpelicans/tictactoe-autumn-2019.git
git push origin master
```

**Attendees:**

|name|status|email|phone
|---|---|---|---|
|Alexandre Gaulet|RP|alexandre.gaulet@redpelicans.com (gauletalexmarvin@gmail.com)|-|
|Marvin Gaulet|RP|marvin.gaulet@redpelicans.com (-)|-|
|Samer Salmi|TN|samersalmi@rocketmail.com|-|
|Aladin Mrebai|TN|aladinmrebai@gmail.com|-|

#### week1

**day 1**
- [ ] [client introduction](https://docs.google.com/presentation/d/1R48RLleag1PTSy4-CzMdhlr02yTUp2JTGXdstxGfFMU/edit#slide=id.g145b507c17_0_109)
- [ ] [boilerplate introduction](https://github.com/facebook/create-react-app), [semver](https://semver.org/)
- [ ] setup boilerplate (single repository with a develop branch), with linter and prettier
- [ ] [git introduction](http://nvie.com/posts/a-successful-git-branching-model/)
- [ ] dummy pull request with feature branch
- [ ] read [react documentation](https://reactjs.org/docs/hello-world.html) (quick start)
- [ ] read [react-elements-vs-react-components](https://medium.freecodecamp.org/react-elements-vs-react-components-fdc776705880)

**day 2**
- [ ] questions on day 1:
  - difference between `React.Element` and `React.Component`
  - how to fix a bug in production (git)
  - Can we modify props within a Component?
- [ ] es6-import-export
  - [cheatsheet](https://hackernoon.com/import-export-default-require-commandjs-javascript-nodejs-es6-vs-cheatsheet-different-tutorial-example-5a321738b50f)
  - [value-import-export](http://es6-features.org/#ValueExportImport)
  - [default-and-wildcard](http://es6-features.org/#DefaultWildcard)
- [ ] react properties, rest parameter, react `PropTypes`
  - [typechecking-with-proptypes](https://reactjs.org/docs/typechecking-with-proptypes.html)
  - [rest-parameter](http://es6-features.org/#RestParameter)
  - [spread-operator](http://es6-features.org/#SpreadOperator)
  - [destructuring](http://es6-features.org/#ParameterContextMatching)
- [ ] [katas](http://es6katas.org/) (modules, spread, rest, destructuring)

**day 3**
- [ ] [autoprefixer](https://github.com/postcss/autoprefixer), [show webpack diagram](https://docs.google.com/presentation/d/1R48RLleag1PTSy4-CzMdhlr02yTUp2JTGXdstxGfFMU/edit#slide=id.g145b507c17_0_109)
- [ ] ways to style in react:
  - css stylesheets (webpack import, className attribute)
  - react style (style attribute, scoped, just JS)
  - [classnames](https://github.com/JedWatson/classnames)
  - [css-modules](https://github.com/css-modules/css-modules)
  - [MUI](https://material-ui.com/getting-started/usage/)
- [ ] craft history (stateless, no props)
- [ ] [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [ ] conception of UI (declarative way)
- [ ] craft cards

**day 4**
- [ ] Add MUI in project
- [ ] explainWebpackDevServer, bundle.js, css , how App is launched
- [ ] craft cards with MUI

**day 5**
- [ ] introduce composability (header with children)
