#  Text format struct

- Every char is mapped to a `uint16` short value, corresponding to SHIFT-JIS / unicode characters used by the game. Uses VWF in 2 types: `12x24px` (halfwidth chars) / `24x24px` (wide chars).

- Regular text box holds a maximum of `3 text lines`.

- `Each line` can be `480 px wide max`, after that next char will automatically `wrap` to the next line.

# Table

You can find the complete table with up-to-date values [HERE](https://github.com/NaomiMod/Rent-A-Hero-No1/blob/main/rtable.txt)


Other than text, control codes provide additional formatting / flags / effects:


# Control codes

|Value|Description|
|-------|------------|
|0x0180|  Return, next row|
|0x0280|  Clear all text *|
|0xa74d|	SPACE (12px)|
|0x504e|	SPACE (12px)|
|0x0000|  SPACE (24px)|
|0x0080|  End of sequence|

*Used to display long text continuously.

# Special Effects & Global Values

|Value|Description|
|-------|------------|
|0x0097|SHAKE TEXT|
|0x0380|TEXT_PAUSE|
|0x0082|TEXT_WHITE|
|0x0182|TEXT_GREEN|
|0x0282|TEXT_BLUE|
|0x0382|TEXT_DARK_GREEN|
|0x0686|SKIP_CHAR|
|0x1088|MONEY_VALUE|
|0x5088|BATTLES_WON|
|0x5188|BATTLES_LOST|
|0x6288|UNK_VALUE3|
|0x6388|UNK_VALUE4|
|0x6788|UNK_VALUE5|
|0x0190|HERO_FIRST_NAME|
|0x0290|HERO_LAST_NAME|
|0x0390|HERO_FIRST_NAME|
|0x0490|HERO_LAST_NAME|
|0x0590|UNK_VALUE1|
|0x0690|UNK_VALUE2|
|0x0092|UNK_VALUE6|
|0x0192|LINK_銀紙鉄道の夜1_NO_STOP|
|0x0292|LINK_銀紙鉄道の夜1_NO_STOP|
|0x0792|UNK_VALUE7|
|0x0892|LINK_ENTER_YOUR_FIRST_NAME_NO_STOP|
|0x0094|ENERGY_DRINK|
|0x10A0|ENERGY_DRINK|
|0x06C0|LINK_PLEASE_ENTER_FIRST_NAME|
|0x09C0|LINK_PLEASE_ENTER_LAST_NAME|
|0x0CC0|LINK_PLEASE_ENTER_FIRST_NAME|
|0x0DC0|LINK_PLEASE_ENTER_LAST_NAME|
|0x0EC0|LINK_PLEASE_ENTER_HERO_NAME|
|0x0FC0|LINK_IS_THIS_OK?|
|0x19C0|LINK_ENTER_THE_ALPHABET|
|0x1BC0|LINK_IF_YOU_WANT_TO_ADD_NEW_LETTER






