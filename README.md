# jQuery DragNDrop
Enable drag and drop functionality on a list of elements.

## Support
I only provide limited support through the Github Issues area.  DO NOT ask for support via email, socialmedia, or other means.  Also check the closed issues before opening a new issue.

## Design Methodology
This plugin is not meant to be a full featured drag & drop plugin.  I envision this as a plugin that contains a base set of features that can be enhanced using callbacks by the developer.  Because of this I am hesitant on adding functionality but am open to adding callbacks where it makes sense.  But feel free to open an [issue](https://github.com/nobleclem/jQuery-DragNDrop/issues) and suggest a feature request if you feel that most people will benefit from it.

## Demo
http://springstubbe.us/projects/jquery-dragndrop/

## Usage
```
$('ul').dragndrop();
$('ul').dragndrop('unload');
$('ul').dragndrop('reload');
$('ul').dragndrop({
    onDrop: function( element, droppedElement ){}
});
```

### Options
| Option            | Values   | Default   | Description                      |
| ----------------- | -------- | --------- | -------------------------------- |
| loadStyles        | bool     | true      | load the default styles          |
| dragElemSelector  | string   | > *       | what elements are draggable      |
| onDrop            | function |           | fires when an element is dropped |


### Methods
**unload**
Disable the jQuery Drag & Drop functionality.

**reload**
Reload the jQuery Drag & Drop functionality.  Useful if you dynamically add/remove items to be dragged and dropped.

**reset**
Reset elements back to their original position when page loaded.
NOT YET IMPLEMENTED


### Callbacks
**onDrop**

Fires after element is dropped into its new position.

`onDrop( element, droppedElement )`

element: The original element targeted for .dragndrop().

droppedElement: The element that was moved.
