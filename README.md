# cli-babel-node
Run es6 from the command line

## Usage
```
npm install
npm run babel-node -- -e "console.log(42)"
```

## Usage with vim, tmux and tmuxify
Be sure you are in a tmux session, then do:

```
vim ./foo.js
:TxRun
TxRun> npm run babel-node -- %
```

Now each time you run `:TxRun` or the default mapping `<leader>mr`, it will
send the current file to babel-node.

## Usage with the babel-node REPL
```
:TxCreate
" Run npm run babel-node in the tmux split.
" Select some code you wish to send to the REPL.
" Do <leader>ms in normal mode.
```
