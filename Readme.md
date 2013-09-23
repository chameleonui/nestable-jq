
# Nestable-jq

  Drag & drop hierarchical list based on [Nestable by David Bushell](https://github.com/dbushell/Nestable)

## Installation

  Install with [component](https://github.com/component/component)

    $ component install chameleonui/nestable-jq

## API

### Options/Defaults

```js
var defaults = {
    listNodeName    : 'ol',
    itemNodeName    : 'li',
    rootClass       : 'dd',
    listClass       : 'dd-list',
    itemClass       : 'dd-item',
    dragClass       : 'dd-dragel',
    handleClass     : 'dd-handle',
    collapsedClass  : 'dd-collapsed',
    placeClass      : 'dd-placeholder',
    noDragClass     : 'dd-nodrag',
    emptyClass      : 'dd-empty',
    expandBtnHTML   : '<button data-action="expand" type="button">Expand</button>',
    collapseBtnHTML : '<button data-action="collapse" type="button">Collapse</button>',
    group           : 0,
    maxDepth        : 5,
    threshold       : 20
};
```
### new Nestable(element, options)

```js
var Nestable = require('nestable-jq');
var n3 = new Nestable('#nestable3');
var n2 = new Nestable('#nestable2', { group: 1 });
var n1 = new Nestable('#nestable1', { group: 1 }).collapseAll();
```

### #.collapseAll()

Collapse all nodes

### #.cExpandAll()

Expand all nodes



## Author(s)

Edgedesign s.r.o. – [Tomas Kuba](https://github.com/tomaskuba)
Based on [Nestable by David Bushell](https://github.com/dbushell/Nestable)

## License

The MIT License (MIT)

Copyright © 2013 Edgedesign s.r.o.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.