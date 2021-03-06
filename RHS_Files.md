# Mail .RHS Files

RHS archives concatenate multiple text chunks, each one simplified as follows:

`POINTERS CHUNK SIZE` --> `TEXT CHUNK DATA SIZE` --> `TEXT POINTER LIST` --> `TEXT DATA` --> `CHUNK END`

- `TEXT POINTERS CHUNK SIZE`: Total size of `TEXT POINTER LIST` chunk
- `TEXT CHUNK DATA SIZE`: Total size of `TEXT DATA` size, multiplied by `0x2`.
- `TEXT POINTER LIST` : An array of `uint16` short values, representing each dialogue relative offset, starting from own `TEXT DATA` multiplied by `0x2`.
- `TEXT DATA` : Game text using Rent a Hero [Text Format Struct](TEXT_Format.md) . *Except for `Chunk 3`* having special delims.
- `CHUNK END`: A fixed string `\x00\x00`.

# Chunk Struct:

|Address|Length|Description|
|-------|------|-----------|
|0x00|0x04|TEXT POINTERS CHUNK SIZE |
|0x04|0x04|TEXT CHUNK DATA SIZE|
|0x08|VAR|TEXT POINTER LIST|
|VAR|VAR|TEXT DATA       |
|VAR|0x02|CHUNK END string: `\x00\x00`|

# Chunk 3 Special Delims:

Used to build a scrollable page by concatenating multiple lines.

|Value|Length|Description|
|-------|------|-----------|
|`\x60\x00\x60\x00`|0x4| USED AT START / END OF `TEXT DATA` |
|`\x60\x00`|0x2|START CONCATENATING NEW LINES`\x60\x00`|

Example:

- TEXT DATA START : `\x60\x00\x60\x00` --> `TEXT 1` --> `TEXT 2` --> `TEXT 3`
- CONCATENATE FOLLOWING LINES: `\x60\x00`, `TEXT 4`--> `TEXT 5`,`TEXT 6`...
- TEXT DATA END: `TEXT 98` --> `TEXT 99` --> `TEXT 100`, --> `\x60\x00\x60\x00`







