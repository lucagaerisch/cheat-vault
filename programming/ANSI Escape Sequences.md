# ANSI Escape Sequences

Sequence starting with - `ESC`

- Octal: `\033`
- Unicode: `\u001b`
- Hexadecimal: `\x1B`

Arguments are delimited by semi colon (`;`).
For example:

```
\033[1;36m  # Set style to bold, cyan foreground.
```

## Terminal Modes

| ESC Code Sequence | Reset Sequence | Description                 |
| ----------------- | -------------- | --------------------------- |
| `ESC[1;34;{...}m` |                | set modes, separated by `;` |
| `ESC[0m`          |                | set all modes               |
| `ESC[1m`          | `ESC[22m`      | set bold mode               |
| `ESC[2m`          | `ESC[22m`      | set dim/faint mode          |
| `ESC[3m`          | `ESC[23m`      | set italic mode             |
| `ESC[4m`          | `ESC[24m`      | set underline mode          |
| `ESC[5m`          | `ESC[25m`      | set blinking mode           |
| `ESC[7m`          | `ESC[27m`      | set inverse/traverse mode   |
| `ESC[8m`          | `ESC[28m`      | set hidden/invisible mode   |
| `ESC[9m`          | `ESC[29m`      | set strikethrough mode      |

> **Note:** Some terminals may not support some of the mode sequences listed above.  

## Color-Codes

Most terminals support from 8 to 16 colors, as well as 256 (8-Bit) colors. These colors can be set by the user and have commonly defined meanings.

### 256 (8-Bit) Colors

| ESC Code Sequence | Description           |
|:----------------- |:--------------------- |
| `ESC[38;5;{ID}m`  | Set foreground color. |
| `ESC[48;5;{ID}m`  | Set background color. |

Where `{ID}` should be replaced with the color index 0 to 255 of the following table:  

![[ansi-colors-256.png]]

### RGB-Colors

More modern terminals supports [Truecolor](https://en.wikipedia.org/wiki/Color_depth#True_color_.2824-bit.29) (24-bit RGB), which allows you to set foreground and background colors using RGB.

| ESC Code Sequence       | Description                  |
|:----------------------- |:---------------------------- |
| `ESC[38;2;{r};{g};{b}m` | set foreground color as RGB. |
| `ESC[48;2;{r};{g};{b}m` | set background color as RGB. |

> **Note:** `38;` and `48;` corresponds to the 16 color sequence and is interpreted by the terminal to set the foreground and background color respectively. Where as `;2` and `;5` sets the color format.

## Cursor Controls

| Sequence                                           | Description                                            |
| -------------------------------------------------- | ------------------------------------------------------ |
| `ESC[H`                                            | moves cursor to home position (0, 0)                   |
| `ESC[{line};{column}H` <br> `ESC[{line};{column}f` | moves cursor to line %, column %                       |
| `ESC[%A`                                           | moves cursor up % lines                                |
| `ESC[%B`                                           | moves cursor down % lines                              |
| `ESC[%C`                                           | moves cursor right % columns                           |
| `ESC[%D`                                           | moves cursor left % columns                            |
| `ESC[%E`                                           | moves cursor to beginning of next line, % lines down   |
| `ESC[%F`                                           | moves cursor to beginning of previous line, % lines up |
| `ESC[%G`                                           | moves cursor to column %                               |
| `ESC[6n`                                           | request cursor position (reports as `ESC[%;%R`)        |
| `ESC M`                                            | moves cursor one line up, scrolling if needed          |
| `ESC 7`                                            | save cursor position (DEC)                             |
| `ESC 8`                                            | restores the cursor to the last saved position (DEC)   |
| `ESC[s`                                            | save cursor position (SCO)                             |
| `ESC[u`                                            | restores the cursor to the last saved position (SCO)   |

### Common Private Modes

These are some examples of private modes, which are not defined by the specification, but are implemented in most terminals.

| ESC Code Sequence | Description                     |
|:----------------- |:------------------------------- |
| `ESC[?25l`        | make cursor invisible           |
| `ESC[?25h`        | make cursor visible             |
| `ESC[?47l`        | restore screen                  |
| `ESC[?47h`        | save screen                     |
| `ESC[?1049h`      | enables the alternative buffer  |
| `ESC[?1049l`      | disables the alternative buffer |
  
[XTerm Sequences](https://invisible-island.net/xterm/ctlseqs/ctlseqs.html) for more private modes defined by XTerm.

> **Note:** These modes may not work in every terminal.


## Keyboard strings

Codes divided by `;` return 2 values when read, eg.  

```cpp
int i = _getch; // when (UP ARROW) pressed
cout << i; // prints 24473
```

| Key                  |   Code   | SHIFT+code | CTRL+code | ALT+code  |
| -------------------- |:--------:|:----------:|:---------:|:---------:|
| F1                   |   0;59   |    0;84    |   0;94    |   0;104   |
| F2                   |   0;60   |    0;85    |   0;95    |   0;105   |
| F3                   |   0;61   |    0;86    |   0;96    |   0;106   |
| F4                   |   0;62   |    0;87    |   0;97    |   0;107   |
| F5                   |   0;63   |    0;88    |   0;98    |   0;108   |
| F6                   |   0;64   |    0;89    |   0;99    |   0;109   |
| F7                   |   0;65   |    0;90    |   0;100   |   0;110   |
| F8                   |   0;66   |    0;91    |   0;101   |   0;111   |
| F9                   |   0;67   |    0;92    |   0;102   |   0;112   |
| F10                  |   0;68   |    0;93    |   0;103   |   0;113   |
| F11                  |  0;133   |   0;135    |   0;137   |   0;139   |
| F12                  |  0;134   |   0;136    |   0;138   |   0;140   |
| HOME (numpad)        |   0;71   |     55     |   0;119   |    \--    |
| UP ARROW (numpad)    |   0;72   |     56     |  (0;141)  |    \--    |
| PAGE UP (numpad)     |   0;73   |     57     |   0;132   |    \--    |
| LEFT ARROW (numpad)  |   0;75   |     52     |   0;115   |    \--    |
| RIGHT ARROW (numpad) |   0;77   |     54     |   0;116   |    \--    |
| END (numpad)         |   0;79   |     49     |   0;117   |    \--    |
| DOWN ARROW (numpad)  |   0;80   |     50     |  (0;145)  |    \--    |
| PAGE DOWN (numpad)   |   0;81   |     51     |   0;118   |    \--    |
| INSERT (numpad)      |   0;82   |     48     |  (0;146)  |    \--    |
| DELETE (numpad)      |   0;83   |     46     |  (0;147)  |    \--    |
| HOME                 | (224;71) |  (224;71)  | (224;119) | (224;151) |
| UP ARROW             | (224;72) |  (224;72)  | (224;141) | (224;152) |
| PAGE UP              | (224;73) |  (224;73)  | (224;132) | (224;153) |
| LEFT ARROW           | (224;75) |  (224;75)  | (224;115) | (224;155) |
| RIGHT ARROW          | (224;77) |  (224;77)  | (224;116) | (224;157) |
| END                  | (224;79) |  (224;79)  | (224;117) | (224;159) |
| DOWN ARROW           | (224;80) |  (224;80)  | (224;145) | (224;154) |
| PAGE DOWN            | (224;81) |  (224;81)  | (224;118) | (224;161) |
| INSERT               | (224;82) |  (224;82)  | (224;146) | (224;162) |
| DELETE               | (224;83) |  (224;83)  | (224;147) | (224;163) |
| PRINT SCREEN         |   \--    |    \--     |   0;114   |    \--    |
| PAUSE/BREAK          |   \--    |    \--     |    0;0    |    \--    |
| BACKSPACE            |    8     |     8      |    127    |    (0)    |
| ENTER                |    13    |    \--     |    10     |    (0     |
| TAB                  |    9     |    0;15    |  (0;148)  |  (0;165)  |
| NULL                 |   0;3    |    \--     |    \--    |    \--    |
| A                    |    97    |     65     |     1     |   0;30    |
| B                    |    98    |     66     |     2     |   0;48    |
| C                    |    99    |     66     |     3     |   0;46    |
| D                    |   100    |     68     |     4     |   0;32    |
| E                    |   101    |     69     |     5     |   0;18    |
| F                    |   102    |     70     |     6     |   0;33    |
| G                    |   103    |     71     |     7     |   0;34    |
| H                    |   104    |     72     |     8     |   0;35    |
| I                    |   105    |     73     |     9     |   0;23    |
| J                    |   106    |     74     |    10     |   0;36    |
| K                    |   107    |     75     |    11     |   0;37    |
| L                    |   108    |     76     |    12     |   0;38    |
| M                    |   109    |     77     |    13     |   0;50    |
| N                    |   110    |     78     |    14     |   0;49    |
| O                    |   111    |     79     |    15     |   0;24    |
| P                    |   112    |     80     |    16     |   0;25    |
| Q                    |   113    |     81     |    17     |   0;16    |
| R                    |   114    |     82     |    18     |   0;19    |
| S                    |   115    |     83     |    19     |   0;31    |
| T                    |   116    |     84     |    20     |   0;20    |
| U                    |   117    |     85     |    21     |   0;22    |
| V                    |   118    |     86     |    22     |   0;47    |
| W                    |   119    |     87     |    23     |   0;17    |
| X                    |   120    |     88     |    24     |   0;45    |
| Y                    |   121    |     89     |    25     |   0;21    |
| Z                    |   122    |     90     |    26     |   0;44    |
| 1                    |    49    |     33     |    \--    |   0;120   |
| 2                    |    50    |     64     |     0     |   0;121   |
| 3                    |    51    |     35     |    \--    |   0;122   |
| 4                    |    52    |     36     |    \--    |   0;123   |
| 5                    |    53    |     37     |    \--    |   0;124   |
| 6                    |    54    |     94     |    30     |   0;125   |
| 7                    |    55    |     38     |    \--    |   0;126   |
| 8                    |    56    |     42     |    \--    |   0;126   |
| 9                    |    57    |     40     |    \--    |   0;127   |
| 0                    |    48    |     41     |    \--    |   0;129   |
| \-                   |    45    |     95     |    31     |   0;130   |
| \=                   |    61    |     43     |   \---    |   0;131   |
| \[                   |    91    |    123     |    27     |   0;26    |
| \]                   |    93    |    125     |    29     |   0;27    |
|                      |    92    |    124     |    28     |   0;43    |
| ;                    |    59    |     58     |    \--    |   0;39    |
| '                    |    39    |     34     |    \--    |   0;40    |
| ,                    |    44    |     60     |    \--    |   0;51    |
| .                    |    46    |     62     |    \--    |   0;52    |
| /                    |    47    |     63     |    \--    |   0;53    |
| \`                   |    96    |    126     |    \--    |  (0;41)   |
| ENTER (numpad)       |    13    |    \--     |    10     |  (0;166)  |
| / (numpad)           |    47    |     47     |  (0;142)  |  (0;74)   |
| \* (numpad)          |    42    |  (0;144)   |  (0;78)   |    \--    |
| \- (numpad)          |    45    |     45     |  (0;149)  |  (0;164)  |
| \+ (numpad)          |    43    |     43     |  (0;150)  |  (0;55)   |
| 5 (numpad)           |  (0;76)  |     53     |  (0;143)  |    \--    |

---

#ANSI

## Resources

- [Wikipedia: ANSI escape code](https://en.wikipedia.org/wiki/ANSI_escape_code)
- [XTerm Sequences](https://invisible-island.net/xterm/ctlseqs/ctlseqs.html)