# Jest Algorithm Testing

This repository provides a steamlined setup for testing algorithms using Jest, a JavaScript testing framework. It is designed for developers looking to practice algorithm implementation and testing effeciently.

## Features

- Pre-configured Jest environment
- Sample alogrithm with tests for quick setup
- Easy to extend for new algorithms

## Prerequisites

Ensure you have the following installed:

- Node.js
- npm or preferred package manager

## Getting Started

1. Clone the repository

```bash
git clone https://github.com/ericstober/jest-algorithm-testing.git
cd jest-algorithm-testing
```

2. Install dependencies

```bash
npm install
```

3. Run tests

```bash
npm test
```

## Project Structure

```
jest-algorithm-testing/
├── algorithms/
│   ├── exampleAlgorithm.js   # Sample algorithm implementation
├── tests/
│   ├── exampleAlgorithm.test.js # Jest test file for the sample algorithm
├── package.json              # Project configuration and dependencies
├── jest.config.js            # Jest configuration file
└── README.md                 # Project documentation
```

## Write Your Own Algorithm

1. Create a new file e.g., `myAlgorithm.js`.
2. Implement your algorithm as a function and export it.
3. Create a corresponding test file, e.g., `myAlgorithm.test.js`.
4. Write your test cases using Jest syntax

Example:

**myAlgorithm.js**

```js
function myAlgorithm(arr) {
  return arr.sort((a, b) => a - b);
}
module.exports = myAlgorithm;
```

**myAlgorithm.test.js**

```js
const myAlgorithm = require("./myAlgorithm");

describe("myAlgorithm", () => {
  test("sorts an array of numbers", () => {
    expect(myAlgorithm([3, 1, 2])).toEqual([1, 2, 3]);
  });
});
```

Run your tests:

```bash
npm test
```

## Acknowledgements

- [Jest](https://jestjs.io/) for providing a robust testing framework.
