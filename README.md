# browser-fft

A cheap FFT by abusing the web audio API

## Example

```js
var FFT = require("browser-fft")

var bufferSize = 2048
var analyse = FFT(bufferSize)
var data = new Float32Array(bufferSize)

for (var i = 0; i < bufferSize; i++) {
    data[i] = Math.random()
}

analyse(data, function (err, value) {
    if (err) {
        console.error(err)
    } else {
        console.log(value)
    }
})
```

## Installation

`npm install browser-fft`

## Contributors

 - Matt-Esch

## MIT Licenced
