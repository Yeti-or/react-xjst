# DEPRECATED: react-xjst

[![Build Status](https://travis-ci.org/awinogradov/react-xjst.svg?branch=master)](https://travis-ci.org/awinogradov/react-xjst)


Virtual DOM provider for XJST. But the better way is https://github.com/awinogradov/ddsl-react.

## Getting Started
Install the module with: `npm install --save react-xjst`

``` jsx
var React = require('react');
var ReactDOM = require('react-dom');

var xjstAdapter = require('react-xjst');
xjstAdapter.use(require('./templates.ddsl.js'), React);

class MyComponent extends React.Component {
    render() {
      return xjstAdapter.provide({
          block: 'my-block'
      });
    }
}

ReactDOM.render(<MyComponent />, document.getElementById('root'));
```

## License MIT
