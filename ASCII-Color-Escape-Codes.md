## Standard escape codes are prefixed with Escape:
|Ctrl-Key|Octal|Unicode|Hexadecimal|Decimal|
|:--:|:---:|:---:|:---:|:---:|
|`^[`|`\033`|`\u001b`|`\x1B`|`27`|

Followed by the command, somtimes delimited by opening square bracket ([), known as a Control Sequence Introducer (CSI), optionally followed by arguments and the command itself.

Arguments are delimeted by semi colon (;).


## Examples:

- `\x1b[1;31m Hello World \x1b[0m`  # Set style to **bold**, *red foreground* then reset.
- `\x1b[2;37;41m Hello World \x1b[0m`  # Set style to **dimmed white foreground** with *red background* then reset.
- `\033[32m Hello World \033[0m`  # Set style to **green font** then reset color.


## Color Codes

| Color Name | Foreground Color Code | Background Color Code |---| Style Code | Style Description |
|:---:|:---:|:---:|:---:|:---:|:---:|
| Black |	30	| 40 |---| 0 | reset all modes (styles and colors) |
| Red	| 31	| 41 |---|  1 | set bold mode. |
| Green |	32	| 42 |---| 2 | set dim/faint mode. |
| Yellow |	33 |	43 |---| 3 | set italic mode. |
| Blue	| 34	| 44 |---| 4 | set underline mode. |
| Magenta	| 35	| 45 |---| 5 | set blinking mode. |
| Cyan	| 36	| 46 |---| 7 | set inverse/reverse mode. |
| White	| 37 |	47 |---| 8 | set hidden/invisible mode. |
| Default	| 39	| 49 |---| 9 |	set strikethrough mode. |
| Bright Black | 90 |	100 |---|---|---|
| Bright Red | 91	| 101 |---|---|---|
| Bright Green |92 | 102 |---|---|---|
| Bright Yellow |	93 | 103 |---|---|---|
| Bright Blue | 94 | 104 |---|---|---|
| Bright Magenta | 95 | 105 |---|---|---|
| Bright Cyan |	96 | 106 |---|---|---|
| Bright White | 97 |	107 |---|---|---|


