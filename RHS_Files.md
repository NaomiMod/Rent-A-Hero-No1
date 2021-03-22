# Mail .RHS Files Struct - WIP

RHS archives concatenate multiple text chunks, each chunk structure could be simplified as follows:

`TEXT TOTAL LINES` --> `TEXT DATA SIZE` --> `TEXT HEADER LIST` --> `TEXT DATA` --> `END OF CHUNK`

- `TOTAL LINES`: Total number of text lines in `TEXT DATA` chunk
- `TEXT DATA SIZE`: Total size of TEXT DATA / size multiplied by `0x2`.
- `TEXT DATA` : Game text using Rent a Hero [Text Format Struct](TEXT_Format.md) . Except for`FANMAILLIST.RHS` Chunk 3 having special delims.
- `TEXT HEADER LIST` : An array of `uint16` short values, representing each dialogue offset, starting from `TEXT DATA` multiplied by `0x2`.
- `CHUNK END`: A fixed string `\x00\x00`.

# Chunk Struct:

|Address|Length|Description|
|-------|------|-----------|
|0x00|0x04|TEXT TOTAL LINES|
|0x04|0x04|TEXT DATA SIZE|
|0x08|VAR|TEXT HEADER LIST|
|VAR|VAR|TEXT DATA       |
|VAR|0x02|CHUNK END string: `\x00\x00`|

# Special Delims:

Used to build a scrollable page by concatenating multiple lines.

|Value|Length|Description|
|-------|------|-----------|
|`\x60\x00`|0x2|EXTRA DELIM USED AT START / END OF A SCROLLABLE CHUNK|
|`\x60\x00`|0x2|CONCATENATE FOLLOWING LINES UNTIL NEXT`\x60\x00`|










