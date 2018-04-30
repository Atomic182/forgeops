# ForgeOps smoke test suite
## Introduction
This suite serves as post-commit test suite.
This is going to cover all 4 major products as well as various parts.

## Setup postcommit tests
Modify config.sh to contain host and port for specific product.
This is still TBD as it dependes on CI/CD system we will use.
Will be finished later to fit our needs.

## Tests
Each test should cover following:
 - Ping test: Is product deployed and running?
 - Login test(Where possible)
 - Successful config import test(custom auth chain, etc... where possible)

### AM
- Ping test
- Login test
- User login test

### DJ
- ?

### IDM
- Ping test
- Login test
- CRUD tests

### IG
- Ping test

## Run tests
To run tests simply execute `./forgeops-smoke-test.sh -l` to see list
of available tests. Select test you want to run and pass it as argument.

For example to run AM smoke test, execute `./forgeops-smoke-test.sh -s am-smoke.sh`
