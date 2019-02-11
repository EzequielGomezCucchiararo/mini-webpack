# OWN WEBPACK BUNDLER

Ronen Amiel live coding tutorial: https://www.youtube.com/watch?v=Gc9-7PBqOC8
Github Repo: https://github.com/ronami/minipack

## What is a bundler
The main goal of a bundler is that let us write modules that work in the browser.

1. EcmaScript Modules (import/export)
2. CommonJs Modules (require/module.exports)

All start from an "entry file" and follow all the dependencies making a dependency graph.

## Implementation overview
1. Parse a single file and extract its dependencies
2. Recursively build a dependency graph
3. Package everything into a single file

### In this project
entry.js > message.js > name.js

### AST Explorer (abstract syntax tree): https://astexplorer.net/
### Babylon: https://www.npmjs.com/package/babylon
Babylon is a JavaScript parser used in Babel that generates AST according to Babel AST format. 
