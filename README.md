| Linux | Windows | MacOS|
|-------|-------|-------|
| ![](https://github.com/rebelware/fibonacci-generator/workflows/node-ci/badge.svg)  | ![](https://github.com/rebelware/fibonacci-generator/workflows/node-ci/badge.svg) | ![](https://github.com/rebelware/fibonacci-generator/workflows/node-ci/badge.svg) |
# fib-tools

## Get the nth Number in the series

```javascript
const {getNumber} = require('@bbq-beets/fib-tools')
assert.strictEqual(getNumber(8), 21)
```

## Get a List of Numbers

```javascript
const {getList} = require('@bbq-beets/fib-tools')
assert.strictDeepEqual(getList(8), [0, 1, 1, 2, 3, 5, 8, 13, 21])
```

## Get a Sequence of Numbers   

```javascript   
const {getSequence} = require('@bbq-beets/fib-tools')

const seq = getSequence()

for (const n of seq) {
  console.log(n) // The next Fibonacci number in the sequence
}
```
## Code Scanning Demo

This repository demonstrates an instance of CWE-020: Improper Imput Validation. 

1. Run through the setup flow in the security tab to enable code scanning. Commit directly to master. 
2. Go to actions, and confirm that the analysis has run successfully.
3. Edit script.js and add this code snippet. Create a PR. Wait for validation. 

```js

function endsWith(x, y) {
  return x.lastIndexOf(y) === x.length - y.length;
}

```
