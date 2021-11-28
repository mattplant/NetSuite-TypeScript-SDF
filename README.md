# NetSuite TypeScript SDF Project Template

## Requirements
- Node - https://nodejs.org/
- TypeScript - https://www.typescriptlang.org/
- Oracle JDK version 11 (64 bit) - required for SuiteCloud SDK
- SuiteCloud SDK - https://github.com/oracle/netsuite-suitecloud-sdk

## Usage

Use this template as a base for your NetSuite TypeScript SDF Projects.

Add your TypeScript files to the */src/TypeScripts* folder.  When *tsc* is executed it will place the corresponding JavaScript file in the */src/FileCabinet/SuiteScripts* directory.

For more info on using TypeScript for NetSuite see https://github.com/headintheclouddev/typings-suitescript-2.0.

### SuiteScript 2.0

This template will compile JavaScript for NetSuite's API Version 2.0 (aka SuiteScript 2.0).

### SuiteCloud SDK

You will need to connect to your NetSuite account.
`suitecloud account:setup`

## Notes

NetSuite customization development is now done with modern tools.  They now support VS Code along with version control systems so that you have complete control over your development processes. Your NetSuite customizations (files, scripts and other custom objects) can be imported and exported between your NetSuite environments (production, sandbox, release preview, or development) and your development environment including detailed deployment logs and audit trails.

This template was initialy built by Oracle's SuiteCloud SDK via `suitecloud project:create -i`.

For TypeScript support I leveraged https://github.com/headintheclouddev/typings-suitescript-2.0.

For linting and automatic code fixing I used https://eslint.org/.

## macOS Tools

Tools I used to fufill the above requirements in macOS.

- Homebrew
  - https://brew.sh/
- Node
  - `brew install node`
- OpenJDK 11
  - `brew install openjdk@11`
- SuiteCloud SDK
  - `npm install -g @oracle/suitecloud-cli`
- VS Code (optional)
  - `brew install --cask visual-studio-code`
- SuiteCloud Extension for VS Code
  - Install the "SuiteCloud Extension for Visual Studio Code" bundle.

