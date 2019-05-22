# New library definitions structure

- @babel/register/index.js.flow

  Reads package name as `@reach/router`

- @reach/router.js.flow

  Reads package name as `@reach/router`

- react-redux/index.js.flow

  Supports multiple-file library definitions
  Supports external imports out of box
  Reads package name `react-redux` from directory name

- redux/index.js.flow

  Supports multiple-file library definitions
  Reads package name `redux` from directory name

- flow-bin.js.flow

  Supports single-file library definitions
  Reads package name `flow-bin` from file name