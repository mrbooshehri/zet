# Fix gibberish bash in vi-mode

Just set the following values in your `.inputrc`

```bash
set vi-cmd-mode-string "\1\e[2 q\2"
set vi-ins-mode-string "\1\e[6 q\2"
```

Tags:
```
#inputrc #bash #gibberish #vi-mode
```

Related:
```
* https://gist.github.com/rej696/59cf458ec8c1487877de203e60d4b4e3 
```
