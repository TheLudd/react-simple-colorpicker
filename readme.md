# React-Simple-ColorPicker

> A simple(r) colorpicker written using React.

A fork of [react-colorpicker](https://github.com/stayradiated/react-colorpicker), but with the extra stuff removed.

## Install

```bash
npm install react-simple-colorpicker --save
```

## Usage

```javascript
var React = require('react');
var ColorPicker = require('react-simple-colorpicker');

var App = React.createClass({

  getInitialState: function() {
    return {
      color : this.props.initialColor
    };
  },

  render: function() {
    return (
      <ColorPicker color={this.state.color} onChange={this.handleChange} />
    );
  },

  handleChange : function(color) {
    console.log(color); // color is a hex string
    this.setState({ color : color });
  }

});

React.render(<App initialColor="#bada55" />, document.body);
```

