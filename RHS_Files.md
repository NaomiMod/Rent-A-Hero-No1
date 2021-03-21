# Mail .RHS Files Struct - WIP

These archives concatenate multiple chunks, each chunk could be simplified as follows:

`TEXT TOTAL LINES` --> `TEXT DATA SIZE` --> `TEXT HEADER LIST` --> `TEXT DATA` --> `\0x00\0x00` (END OF CHUNK)


# Chunk Struct:

|Address|Length|Description|
|-------|------|-----------|
|0x00|0x04|TEXT TOTAL LINES|
|0x04|0x04|TEXT DATA SIZE|
|0x08|VAR|TEXT HEADER LIST|
|VAR|VAR|TEXT DATA       |
|VAR|0x02|CHUNK_END|



- `TOTAL-LINES` : Total number of text lines in `TEXT DATA` chunk
- `TEXT DATA SIZE` Total size of TEXT DATA / siz multiplied by `0x2`.
- `TEXT DATA` : Game text using Rent a Hero [Text Format Struct](TEXT_Format.md).
- `TEXT HEADER LIST` : An array of `uint16` short values, representing each dialogue offset, starting from `TEXT DATA` multiplied by `0x2`.





