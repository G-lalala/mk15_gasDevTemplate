# mk15_gasDevTemplate

This repository is a template for developing Google Apps Script applications.
When you create an app on GAS, you can fork or select this template.
You can use Git for GAS app development and select deployment environments.

## Prerequisites

- Clasp must be installed

## How to Use

1. Clone this repository or select it as a template or fork it
2. Run `npm install`
3. Run `clasp login`
4. If you need to login with another account:
   - Copy `.clasprc.json` to this directory and rename it to `.clasprc-production.json`
   - After running `clasp login`, you will get `.clasprc.json` in your home directory
   - Currently, you cannot push to the staging directory, so please re-login to your default account
5. Run `clasp clone <script ID>`
6. Rename `clasp.json` to `clasp.staging.json` and move `appsscript.json` to `dist/appsscript.json`

You can use the following commands for deployment:

- `npm run stg-push` for staging environment
- `npm run prod-push` for production environment
