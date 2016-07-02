# Griss cells

Cells module for [Griss](https://github.com/battaglr/griss/).

## Overview

Extends [Griss](https://github.com/battaglr/griss/) by adding a set of cell
classes based on fractions —from halves to sixths— and 3 different breakpoints.

Key features:

- Fluid cells based on fractions.
- Responsive and mobile-first.
- Lightweight (~414 bytes minified and gzipped).
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
[Griss core](https://github.com/battaglr/griss/#installation) module.*

## Usage

*Make sure you have read
[Griss core documentation](https://github.com/battaglr/griss/#usage) first.*

Combine the base cell class —`Grid-cell`— with the class that defines the
size you need for your content —i.e. `Grid-cell--size(1/2)`.

#### Examples

Some basic examples:

- A grid using halves:

  ```html
  <div class="Grid">
    <div class="Grid-cell Grid-cell--size(1/2)"> ... </div>
    <div class="Grid-cell Grid-cell--size(1/2)"> ... </div>
  </div>
  ```

- A grid using fifths:

  ```html
  <ul class="Grid">
    <li class="Grid-cell / Grid-cell--size(3/5)"> ... </li>
    <li class="Grid-cell / Grid-cell--size(1/5)"> ... </li>
    <li class="Grid-cell / Grid-cell--size(1/5)"> ... </li>
  </ul>
  ```

- A grid using halves and fifths on different breakpoints:

  ```html
  <div class="Grid">
    <div class="Grid-cell Grid-cell--size(1/2)@s Grid-cell--size(3/5)@m"> ... </div>
    <div class="Grid-cell Grid-cell--size(1/2)@s Grid-cell--size(2/5)@m"> ... </div>
  </div>
  ```

For more examples, please check out the
[test page](https://battaglr.github.io/griss-cells/test/test.html).

#### Available classes

##### Default

- `Grid-cell--size(1/2)`
- `Grid-cell--size(2/2)`
- `Grid-cell--size(1/3)`
- `Grid-cell--size(2/3)`
- `Grid-cell--size(3/3)`
- `Grid-cell--size(1/4)`
- `Grid-cell--size(2/4)`
- `Grid-cell--size(3/4)`
- `Grid-cell--size(4/4)`
- `Grid-cell--size(1/5)`
- `Grid-cell--size(2/5)`
- `Grid-cell--size(3/5)`
- `Grid-cell--size(4/5)`
- `Grid-cell--size(5/5)`
- `Grid-cell--size(1/6)`
- `Grid-cell--size(2/6)`
- `Grid-cell--size(3/6)`
- `Grid-cell--size(4/6)`
- `Grid-cell--size(5/6)`
- `Grid-cell--size(6/6)`

##### Breakpoints

- `Grid-cell--size(n/n)@s`
- `Grid-cell--size(n/n)@m`
- `Grid-cell--size(n/n)@l`

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
