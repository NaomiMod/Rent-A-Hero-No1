# Mail .RHS Files Struct - WIP

These archives concatenate multiple chunks, each chunk composed by: `TOTAL-LINES` - `UNK` - `TEXT HEADER LIST` - `TEXT DATA`  

- `TOTAL-LINES` : Total number of text lines in `TEXT DATA` chunk
- `TEXT HEADER LIST` : An array of `uint16` short values, representing each dialogue offset, starting from `TEXT DATA` multiplied by `0x2`.
- `TEXT DATA` : Game text using Rent a Hero [Text Format Struct](TEXT_Format.md).


|OFFSET|VALUE|
|------|-----|
|`0x0` | TOTAL LINES|
|`0x4` | UNK|

