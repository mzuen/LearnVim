# LearnVim
learning vim step by step

Multi-window
---
```bash
# open one vim editor
vim -o1

# open two vim editors
vim -o2
```


Substitute
---
```bash
vim -c %s/{matches}/{replaceBy}/g {file_name}

vim -c %s/A/B/g test.txt
```

Terms
---
There are three terms in VIM.
- buffer: in-memory space bound with file which open by vim
- window: view part of buffer
- tab: collection of windows


1. buffer
  - vim {file_1} {file2}
  - :ls -> show all the buffers
  - :buffer 2 -> jump to buffer 2
2. window
  - :split {file_2} -> means split herizonally with file2
  - :vsplit {file_2} -> means split veritically with file2
  - (key bind) ctrl+w + [hjkl] -> to jump to target window
3. tab
  - :tabnew file_2 -> mean open a new tab with file2
  - gt -> go to the next tab
  - gT -> go to the previous tab
