*This repository is a mirror of the [component](http://component.io) module [component/flipbox](http://github.com/component/flipbox). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-flipbox`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# flipbox

  Double-sided flip box using css transformations.

## Installation

    $ component install component/flipbox

## Example

```html
<div id="card">
  <div>
    <div>front</div>
    <div>back</div>
  </div>
</div>

<script>
  var card = document.querySelector('#card');
  var Flipbox = require('flipbox');
  var box = new Flipbox(card);

  box.el.onclick = function(){
    box.flip();
  };
</script>
```

## API

### Flipbox(el)

  Initialize a `Flipbox` with the given container `el`. Inside
  this should be a wrapper `div`, within that should be the two
  faces. View _./example.html_ for a full example.

### Flipbox#flip()

  Toggle the visibile face.

### Flipbox#front()

  Show the front face.

### Flipbox#back()

  Show the back face.

## License

  MIT
