---
layout: wiki
title: Vim
categories: Vim
description: Common commands for Vi/Vim editor.
keywords: Vim
---
### Cursor movement ###
#### For character ####

| Func | Key |
|:----|:---:|
| up | k |
| down | j  |
| left | h |
| right | l |

Tip: prefix a cursor movement command with a number to repeat it. For example, 4j moves down 4 lines.

#### For word ####

| Func | Key |
|:----|:---:|
| head | b |
| tail | e |

#### For line ####

| Func | Key |
|:----|:---:|
| head | 0 |
| tail | $ |
| 1st line of doc | gg |
| last line of doc | G |
| line 5 | 5G or 5gg |

#### For screen ####

| Func | Key |
|:----|:---:|
| top | H |
| middle | M |
| bottom | L |
| next screen | Ctrl + f |
| previous screen | Ctrl + b |
| next half screen | Ctrl + d |
| previous half screen | Ctrl + u |

### Insert mode ###
#### Insert ####

| Func | Key |
|:----|:---:|
| insert before the cursor | i |
| insert after the cursor (append) | a |
| append a new line below current line | o |
| append a new line above current line | O |

#### Copy/Cut/Paste/Replace ####

| Func | Key |
|:----|:---:|
| copy word | yiw |
| yank (copy) line | yy |
| yank 2 lines | 2yy |
| cut selected | d |
| cut line | dd |
| paste after cursor | p |
| paste before cursor | P |
| replace all str1 with str2 | :%s/str1/str2/g |
| replace str1 with str2 from line 1 to line 5| :1,5/str1/str2/g |

#### Invert case ####

| Func | Key |
|:----|:---:|
| case invert | ~ |
| to lower case | gu |
| to capital | gU |
| current line to lower case | guu |
| current line to capital | gUU |

#### Search ####

| Func | Key |
|:----|:---:|
| search | /str |
| search backward | ?str |
| next | n |
| next in opposite direction | N |
