# `@schatx/tsconfig`

TSConfig for schatx to extend.

Require `Typescript >= 5.0`. `Node -> NodeNext`. `ECMAScript -> ESNext`

## Installation

```sh
npm install --save-dev @scharx/tsconfig
```

## Usage
Add one of avaiable conifgurations to your `tsconfig.json`:

### The Base Configuration

```json
"extends": "@schatx/tsconfig/tsconfig.json"
```

### Configuration for Browser Environment

```json
"extends": "@schatx/tsconfig/tsconfig.dom.json"
```

### Configuration for Node Environments

First install the types for the Node.js version you are targeting, for example:

```shell
npm install @types/node --save-dev
```

and you need to extend the TSConfig:

```json
"extends": "@schatx/tsconfig/tsconfig.node.json"
```

## Emitting Declaration Files

If you are building a library or a component library, you can enable declaration file emitting by also extending `@schatx/tsconfig/tsconfig.lib.json` in your `tsconfig.json`:

```json
"extends": [
  "@schatx/tsconfig/tsconfig.dom.json",
  "@schatx/tsconfig/tsconfig.lib.json"
]
```
