# codex

#Export VS Code extensions to list

```
code --list-extensions > vscode-extensions.txt 

#Import VS Code extensions on target machine
```
#!/bin/bash
curl https://messaoudim.github.io/codex/vscode-extensions.txt | xargs -L 1 code --install-extension

#Uninstall VS Code extensions from list
```
#!/bin/bash
curl https://messaoudim.github.io/codex/vscode-extensions.txt | xargs -L 1 code --uninstall-extension
```
