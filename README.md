# NetSuite TypeScript SDF Project Template

For an example of this project template being used, see [SuiteTools](https://github.com/mattplant/SuiteTools).

## Requirements

- Node - <https://nodejs.org/>
- TypeScript - <https://www.typescriptlang.org/>
- Oracle JDK version 17 (64 bit) - required for SuiteCloud SDK
- SuiteCloud SDK - <https://github.com/oracle/netsuite-suitecloud-sdk>
- "SuiteCloud Development Integration" (245955) bundle installed in NetSuite

## Initial Setup

These initial steps will only need to be done once.

### Core Configuration

- clone the repo
  - `git clone https://github.com/mattplant/netsuite-typescript-sdf.git`
- enable linting
  - `cd netsuite-typescript-sdf; npm install`
- connect your NetSuite account
  - `suitecloud account:setup`

### VS Code Configuration (optional)

- install VS Code extensions
  - SuiteCloud Extension for Visual Studio Code - <https://marketplace.visualstudio.com/items?itemName=Oracle.suitecloud-vscode-extension>
  - VS Code ESLint extension - <https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint>
  - Prettier ESLint - <https://marketplace.visualstudio.com/items?itemName=rvest.vs-code-prettier-eslint>
- allow VS Code to run tasks automatically so that TypeScript can automatically run in the background
  - in command palette, select "Tasks: Manage Automatic Tasks in Folder" and then "Allow Automatic Tasks in Folder"

## Usage

Now in VS Code when you create your TypeScript files in the */src/TypeScripts/netsuite-typescript-sdf/ folder they will automatically be linted as you type and automatically formatted and code fixed upon saving. The corresponding JavaScript for NetSuite's API Version 2.1 (aka SuiteScript 2.1) will automatically be generated in the*/src/FileCabinet/SuiteScripts/netsuite-typescript-sdf/ folder ready for deployment to your NetSuite account.

## Notes

NetSuite customization development is now done with modern tools. You now have complete control over your development processes including using VS Code. Your NetSuite customizations (files, scripts and other custom objects) can be imported and exported between your NetSuite environments (production, sandbox, release preview, or development).

This template was initially built by Oracle's SuiteCloud SDK via `suitecloud project:create -i`.

For NetSuite TypeScript support I leveraged <https://github.com/headintheclouddev/typings-suitescript-2.0>.

## macOS Tools (optional)

Tools I used to fulfill the above requirements in macOS.

- Homebrew
  - <https://brew.sh/>
- Node
  - `brew install node`
- TypeScript
  - `npm install -g typescript`
- OpenJDK 17
  - `brew install openjdk@17`
- SuiteCloud SDK
  - `npm install -g @oracle/suitecloud-cli`
- VS Code (optional)
  - `brew install --cask visual-studio-code`
- Oracle's SuiteCloud extension for VS Code (optional)
  - [SuiteCloud Extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=Oracle.suitecloud-vscode-extension)
- Microsoft's ESLint extension for VS Code (optional)
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
