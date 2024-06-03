<<<<<<< HEAD
# article-lsp-go-to-definition
# article-lsp-go-to-definition
=======
# LSP Go To Definition

Sample code for the article, Go To Definition in the Language Server Protocol

## Functionality

This Language Server works for a subset of the Kotlin, saved in .mykt files. It has the following language features:
- Completions
- Go To Definition

## Structure

```
.
├── client // Language Client
│   ├── src
│   │   ├── test // End to End tests for Language Client / Server
│   │   └── extension.ts // Language Client entry point
├── package.json // The extension manifest.
└── server // Language Server
    └── src
        └── server.ts // Language Server entry point
```

## Running the Sample

- Run `npm install` in this folder. This installs all necessary npm modules in both the client and server folder
- Open VS Code on this folder.
- Press Ctrl+Shift+B to compile the client and server.
- Switch to the Debug viewlet.
- Select `Launch Client` from the drop down.
- Run the launch config.
- If you want to debug the server as well use the launch configuration `Attach to Server`
- In the [Extension Development Host] instance of VSCode, open a document in 'plain text' language mode.
  - Type `j` or `t` to see `Javascript` and `TypeScript` completion.
  - Enter text content such as `AAA aaa BBB`. The extension will emit diagnostics for all words in all-uppercase.
>>>>>>> 222269450aea57d86a582eae057b5bd9ea537c01
