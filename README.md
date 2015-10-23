# unflex

An even simpler, responsive CSS grid.


## What's this?

__unflex__ is a tiny, responsive, **flex**-based CSS grid system.
The entire `unflex.css` file is 80 bytes minified.


```css
@media (min-width: 640px) {
  .row { display: flex; flex-flow: row wrap;}
  .col { flex-grow: 1 }
}
```

## Why this?

As you might have noticed, __unflex__ is based on
[Chris Nager's __ungrid__](https://github.com/chrisnager/ungrid).

While `display: table-cell` is an effective, simple way of achieving
responsive rows and columns, the properties `table/table-cell` have some
display issues when resizing the browser window---the browser
"lags behind" to display the rows/columns properly. It's just something
I noticed while using __ungrid__ for my work.

This, and the fact that all major browser now support `display: flex`,
is the reason why I created __unflex__. Even though `display: flex` has
many features that make the notion of "rows" and "columns" obsolete,
I think a table-based layout is a simple enough approach for small
projects.


## Getting started

- Just copy and paste the contents of `unflex.min.css` into your CSS file.

## Tutorial

Simply put as many `.col`s as you wish in your `.row`s and the `.col`s
will automatically be evenly spaced. This allows you to roll your own
simple grids.

```html
<div class="row">
    <div class="col">☯</div>
    <div class="col">☯</div>
    <div class="col">☯</div>
    …
    <div class="col">☯</div>
</div>
```

# License

![zlib License](https://img.shields.io/badge/license-zlib-blue.svg)

Copyright (c) 2015 [Eroica](https://github.com/Eroica)

This software is provided 'as-is', without any express or implied
warranty. In no event will the authors be held liable for any damages
arising from the use of this software.

Permission is granted to anyone to use this software for any purpose,
including commercial applications, and to alter it and redistribute it
freely, subject to the following restrictions:

1.	The origin of this software must not be misrepresented; you must
	not claim that you wrote the original software. If you use this
	software in a product, an acknowledgment in the product
	documentation would be appreciated but is not required.
2.	Altered source versions must be plainly marked as such, and must
	not be misrepresented as being the original software.
3.	This notice may not be removed or altered from any source
	distribution.

## ungrid

The original code of __ungrid__ is licensed under the MIT license.

The MIT License (MIT)

Copyright (c) 2014-2015 [Chris Nager](//twitter.com/chrisnager)

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
