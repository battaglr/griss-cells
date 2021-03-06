# Griss cells

Cells module for [Griss](https://github.com/battaglr/griss/).

## Overview

Extends [Griss](https://github.com/battaglr/griss/) by adding a set of cell
classes based on fractions —from halves to sixths— with three available
breakpoints to adjust the size at different screen widths.

Key features:

- Fluid cells based on fractions.
- Responsive and mobile-first.
- Lightweight (~350 bytes minified and gzipped).
- Extensible using the different
  [available modules](https://github.com/battaglr/griss/#available-modules)
  or your own code.

## Installation

Install it using [npm](https://npmjs.com):

```sh
npm install griss-cells
```

Or simply [download the minified file](dist/griss-cells.min.css) and include
it into your project:

```html
<link href="griss-cells.min.css" rel="stylesheet" />
```

*You will also need to install
[Griss core module](https://github.com/battaglr/griss/#installation).*

## Usage

*Make sure you have read
[Griss core documentation](https://github.com/battaglr/griss/#usage) first.*

Combine the base cell class —`gs-Grid-cell`— with the class that defines the
cell size that you need for your content —i.e. `gs-Grid-cell--size(1/2)`.

To define the size of each cell you can choose any fraction from halves to
sixths or use only the base cell class if you want it to be as wide as
its container.

If you need to make adjustments at different screen widths use any of the
available breakpoint suffixes: `@s`, `@m` and `@l` —i.e.
`gs-Grid-cell--size(1/2)@m`.

#### Examples

Some basic examples:

- A grid using halves:

  ```html
  <div class="gs-Grid">
    <div class="gs-Grid-cell gs-Grid-cell--size(1/2)"> ... </div>
    <div class="gs-Grid-cell gs-Grid-cell--size(1/2)"> ... </div>
  </div>
  ```

- A grid using fifths:

  ```html
  <ul class="gs-Grid">
    <li class="gs-Grid-cell gs-Grid-cell--size(3/5)"> ... </li>
    <li class="gs-Grid-cell gs-Grid-cell--size(1/5)"> ... </li>
    <li class="gs-Grid-cell gs-Grid-cell--size(1/5)"> ... </li>
  </ul>
  ```

- A grid using halves and fifths at different breakpoints:

  ```html
  <div class="gs-Grid">
    <div class="gs-Grid-cell gs-Grid-cell--size(1/2)@s Grid-cell--size(3/5)@m"> ... </div>
    <div class="gs-Grid-cell gs-Grid-cell--size(1/2)@s Grid-cell--size(2/5)@m"> ... </div>
  </div>
  ```

For more examples, please check out the
[test page](https://battaglr.github.io/griss-cells/test/test.html).

#### Available classes

##### Base

- `gs-Grid-cell--size(1/2)`
- `gs-Grid-cell--size(1/3)`
- `gs-Grid-cell--size(2/3)`
- `gs-Grid-cell--size(1/4)`
- `gs-Grid-cell--size(2/4)`
- `gs-Grid-cell--size(3/4)`
- `gs-Grid-cell--size(1/5)`
- `gs-Grid-cell--size(2/5)`
- `gs-Grid-cell--size(3/5)`
- `gs-Grid-cell--size(4/5)`
- `gs-Grid-cell--size(1/6)`
- `gs-Grid-cell--size(2/6)`
- `gs-Grid-cell--size(3/6)`
- `gs-Grid-cell--size(4/6)`
- `gs-Grid-cell--size(5/6)`

##### Breakpoints

- `gs-Grid-cell--size(n/n)@s`
- `gs-Grid-cell--size(n/n)@m`
- `gs-Grid-cell--size(n/n)@l`

*`n/n` should be replaced with an available fraction.*

## Browser support

The following browsers are supported:

- Chrome *latest 5*
- Firefox *latest 5*
- Internet Explorer *8+*
- Edge *latest 5*
- Opera *latest 5*
- Safari *latest 5*
- iOS Safari *latest 5*
- Android Browser *2.1+*

*IE8 does not support media queries.*

## Contributing

Contributions are welcome! Please, read the
[contribution guidelines](contributing.md) first.

## License

Released under the [MIT license](license.txt).
