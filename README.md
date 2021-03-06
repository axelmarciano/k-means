# k-means

> K-Means clustering in JavaScript.

[![NPM](https://nodei.co/npm/kmeansjs.png)](https://nodei.co/npm/kmeansjs)

# Demo

[https://lab.miguelmota.com/k-means](https://lab.miguelmota.com/k-means)

# Install

```bash
npm install k-meansjs
```

```bash
bower install kmeans
```

# Usage

Take a look at the [full example][].

```javascript
var KMeans = require('k-meansjs');

var data = [
  [6,5],
  [9,10],
  [10,1],
  [5,5]
  ...
];

var kmeans = KMeans({
  data: data,
  k: 3
});

kmeans.on('iteration', function(self) {
  draw.call(self);
});

kmeans.on('end', function(self) {
  console.log(self.iterations);
});

kmeans.run();
```

# Test

```bash
npm test
```

# License

MIT

[full example]: example/
