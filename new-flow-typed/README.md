# New library definitions structure

- `@babel/register/index.js.flow`

  Reads package name as `@babel/register` from directory name

- `@reach/router.js.flow`

  Reads package name as `@reach/router` from file name

- `react-redux/index.js.flow`

  Supports multiple-file library definitions  
  Supports external imports out of box  
  Reads package name as `react-redux` from directory name

- `redux/index.js.flow`

  Supports multiple-file library definitions  
  Reads package name as `redux` from directory name

- `flow-bin.js.flow`

  Supports single-file library definitions  
  Reads package name as `flow-bin` from file name

# Current equivalent

```ini
[options]
module.name_mapper='@babel/register\(.*\)' -> '<PROJECT_ROOT>/new-flow-typed/@babel/register\1'
module.name_mapper='@reach/router' -> '<PROJECT_ROOT>/new-flow-typed/@reach/router.js.flow'
module.name_mapper='react-redux\(.*\)' -> '<PROJECT_ROOT>/new-flow-typed/react-redux\1'
module.name_mapper='redux\(.*\)' -> '<PROJECT_ROOT>/new-flow-typed/redux\1'
module.name_mapper='redux\(.*\)' -> '<PROJECT_ROOT>/new-flow-typed/redux\1'
module.name_mapper='flow-bin' -> '<PROJECT_ROOT>/new-flow-typed/flow-bin.js.flow\1'

# And so on...
```