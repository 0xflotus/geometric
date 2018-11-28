# geometric
A JavaScript library with geometric functions.

## Installation

### Web browser
In vanilla, a `geometric` global is exported. You can use the latest version from unpkg.
```html
<script src="https://unpkg.com/geometric@0.0.2/build/geometric.js"></script>
<script src="https://unpkg.com/geometric@0.0.2/build/geometric.min.js"></script>
```
If you'd rather host it yourself, download the latest release from the [`build` directory](https://github.com/HarryStevens/geometric/tree/master/build).

### npm

```bash
npm i geometric -S
```
```js
var geometric = require("geometric");
```

## API

<a name="angleDegrees" href="#angleDegrees">#</a> geometric.<b>angleDegrees</b>(<em>a</em>, <em>b</em>)

Calculate the angle between two points, in degrees. Takes two arguments, each of which is a point represented as an array of two numbers, where the first number is its x coordinate and the second number is its y coordinate.

```js
geometric.angleDegrees([0, 0], [1, 0]); // 0
geometric.angleDegrees([0, 0], [-1, 0]); // 180
```

<a name="angleRadians" href="#angleRadians">#</a> geometric.<b>angleRadians</b>(<em>a</em>, <em>b</em>)

Calculate the angle between two points, in [radians](https://en.wikipedia.org/wiki/Radian). Takes two arguments, each of which is a point represented as an array of two numbers, where the first number is its x coordinate and the second number is its y coordinate.

```js
geometric.angleRadians([0, 0], [1, 0]); // 0
geometric.angleRadians([0, 0], [-1, 0]); // Math.PI
```

<a name="distasnce" href="#distasnce">#</a> geometric.<b>distasnce</b>(<em>a</em>, <em>b</em>)

Calculate the distance between two points. Takes two arguments, each of which is a point represented as an array of two numbers, where the first number is its x coordinate and the second number is its y coordinate.

```js
geometric.distance([1, 0], [1, 0]); // 0
geometric.distance([1, 0], [-1, 0]); // 2
```