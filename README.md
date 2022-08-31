Cypress E2E Automation

# Requirements:
- Node.js >v14

# Instructions
1. Clone this repo
2. Navigate to the cloned repo using your terminal and execute `npm install`
3. After installing the dependencies execute the command `npx cypress open` from the directory of the cloned repo

# Possible Errors
It is possible that `npx cypress open` may fail to execute due to cypress verification timeout. In order to fix this, follow these instructions:
1. Navigate to `node_modules\cypress\lib\tasks\verify.js`
2. Search for `VERIFY_TEST_RUNNER_TIMEOUT_MS` and change it from `30000` (default) to `100000`.

