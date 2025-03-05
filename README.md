# deepseek-vscode

Based on this Beyond Fireship video: <https://www.youtube.com/watch?v=clJCDHml2cA>

Notes:

- initialized using `npx --package yo --package generator-code -- yo code` and setting a bunch of things to "deepseek-vscode" and using the `yarn` option

- <https://code.visualstudio.com/api/get-started/your-first-extension>
  - This example uses the default Ctrl+Shift+P command "Hello World"
  - I had to run `tsc` within this project so that it generates `/out/extension.js`, otherwise I either couldn't get the "Hello World" command to run or it got an error.
  - you might want to instead run `tsc --watch` so it automatically updates when you make updates

- <https://ollama.com/library/deepseek-r1:1.5b>

- <https://ollama.com/download>
  - run it and it'll help you install the CLI that works when the ollama app is running, for example, this CLI command: `ollama run deepseek-r1:1.5b`

- but within the project, don't want to interact with cli but rather REST API or JS SDK:
  - `npm install ollama`, or
  - `yarn add ollama`

- using es6-string-html VSCode extension by Tobermory is recommended
