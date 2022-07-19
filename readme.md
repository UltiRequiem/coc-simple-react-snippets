# Simple React Snippets

The essential collection of React Snippets and commands.

## Installation

> Depends on [coc-snippets](https://github.com/neoclide/coc-snippets)

In your (n)vim👇

```
:CocInstall coc-simple-react-snippets coc-snippets
```

## Features

Only what you need and nothing more. **No Redux. No React Native.**

Simply, simple React snippets.

These snippets were selected carefully from my own day-to-day React use. Not
everything in React is included here. This is a hand selected set of snippets
that work the way that you would expect, not just a copy of the documentation.

## Snippets

| Snippet | Renders                                       |
| ------- | --------------------------------------------- |
| `imr`   | Import React                                  |
| `imrc`  | Import React / Component                      |
| `imrd`  | Import ReactDOM                               |
| `imrs`  | Import React / useState                       |
| `imrse` | Import React / useState useEffect             |
| `impt`  | Import PropTypes                              |
| `impc`  | Import React / PureComponent                  |
| `cc`    | Class Component                               |
| `ccc`   | Class Component With Constructor              |
| `cpc`   | Class Pure Component                          |
| `sfc`   | Stateless Function Component                  |
| `cdm`   | componentDidMount                             |
| `uef`   | useEffect Hook                                |
| `cwm`   | componentWillMount                            |
| `cwrp`  | componentWillReceiveProps                     |
| `gds`   | getDerivedStateFromProps                      |
| `scu`   | shouldComponentUpdate                         |
| `cwu`   | componentWillUpdate                           |
| `cdu`   | componentDidUpdate                            |
| `cwu`   | componentWillUpdate                           |
| `cdc`   | componentDidCatch                             |
| `gsbu`  | getSnapshotBeforeUpdate                       |
| `ss`    | setState                                      |
| `ssf`   | Functional setState                           |
| `usf`   | Declare a new state variable using State Hook |
| `ren`   | render                                        |
| `rprop` | Render Prop                                   |
| `hoc`   | Higher Order Component                        |

## Full Expansions

### imr - Import React

```javascript
import * as React from "react";
```

### imrc - Import React, Component

```javascript
import * as React from "react";
import { Component } from "react";
```

### imrd - Import ReactDOM

```javascript
import ReactDOM from "react-dom";
```

### imrs - Import React, useState

```javascript
import * as React from "react";
import { useState } from "react";
```

### imrse - Import React, useState, useEffect

```javascript
import * as React from "react";
import { useEffect, useState } from "react";
```

### impt - Import PropTypes

```javascript
import PropTypes from "prop-types";
```

### impc - Import PureComponent

```javascript
import * as React from "react";
import { PureComponent } from "react";
```

### cc - Class Component

```javascript
class | extends Component {
  state = { | },
  render() {
    return ( | );
  }
}

export default |;
```

### ccc - Class Component With Constructor

```javascript
class | extends Component {
  constructor(props) {
    super(props);
    this.state = { | };
  }
  render() {
    return ( | );
  }
}

export default |;
```

### cpc - Class Pure Component

```javascript
class | extends PureComponent {
  state = { | },
  render() {
    return ( | );
  }
}

export default |;
```

### sfc - Stateless Function Component

```javascript
const | = props => {
  return ( | );
};

export default |;
```

### cdm - componentDidMount

```javascript
componentDidMount() {
  |
}
```

### uef - useEffect Hook

```javascript
useEffect(() => {
  |
}, []);
```

### cwm - componentWillMount

```javascript
//WARNING! To be deprecated in React v17. Use componentDidMount instead.
componentWillMount() {
  |
}
```

### cwrp - componentWillReceiveProps

```javascript
//WARNING! To be deprecated in React v17. Use new lifecycle static getDerivedStateFromProps instead.
componentWillReceiveProps(nextProps) {
  |
}
```

### gds - getDerivedStateFromProps

```javascript
static getDerivedStateFromProps(nextProps, prevState) {
  |
}
```

### scu - shouldComponentUpdate

```javascript
shouldComponentUpdate(nextProps, nextState) {
  |
}
```

### cwu - componentWillUpdate

```javascript
//WARNING! To be deprecated in React v17. Use componentDidUpdate instead.
componentWillUpdate(nextProps, nextState) {
  |
}
```

### cdu - componentDidUpdate

```javascript
componentDidUpdate(prevProps, prevState) {
  |
}
```

### cwun - componentWillUnmount

```javascript
componentWillUnmount() {
  |
}
```

### cdc - componentDidCatch

```javascript
componentDidCatch(error, info) {
  |
}
```

### gsbu - getSnapshotBeforeUpdate

```javascript
getSnapshotBeforeUpdate(prevProps, prevState) {
  |
}
```

### ss - setState

```javascript
this.setState({ | : | });
```

### ssf - Functional setState

```javascript
this.setState(prevState => {
  return { | : prevState.| }
});
```

### usf - Declare a new state variable using State Hook

```javascript
const [|, set|] = useState();
```

_Hit Tab to apply CamelCase to function. e.g. [count, setCount]_

### ren - render

```javascript
render() {
  return (
    |
  );
}
```

### rprop - Render Prop

```javascript
class | extends Component {
  state = { | },
  render() {
    return this.props.render({
      |: this.state.|
    });
  }
}

export default |;
```

### hoc - Higher Order Component

```javascript
function | (|) {
  return class extends Component {
    constructor(props) {
      super(props);
    }

    render() {
      return < | {...this.props} />;
    }
  };
}
```

## Support

Open an Issue, I will check it a soon as possible 👀

If you want to hurry me up a bit
[send me a tweet](https://twitter.com/UltiRequiem) 😆

Consider [supporting me on Patreon](https://patreon.com/UltiRequiem) if you like
my work 🙏

Don't forget to star the repo ⭐

## Licence

Licensed under the MIT License 📄
