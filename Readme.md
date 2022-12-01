# Steps to reproduce

- Use NVM or any other node manager

## Pass
- nvm use 16
- yarn
- yarn test

```
PASS  ./index.spec.js
  ✓ adds 1 + 2 to equal 3 (1 ms)

Test Suites: 1 passed, 1 total
Tests:       1 passed, 1 total
Snapshots:   0 total
Time:        0.271 s, estimated 1 s
````


## Fail
- nvm use 18
- yarn
- yarn test

```
 FAIL  ./index.spec.js
  ● Test suite failed to run

    /Users/sebastian/playground/jest-error/node_modules/node-fetch/src/utils/form-data.js:1
    ReferenceError: Buffer is not defined

      at Object.<anonymous> (node_modules/node-fetch/src/utils/form-data.js:7:24)

Test Suites: 1 failed, 1 total
Tests:       0 total
Snapshots:   0 total
```