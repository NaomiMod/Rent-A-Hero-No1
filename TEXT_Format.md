#  Text format struct

Every char is mapped by a `uint16` short value, corresponding to a ASCII character used by game font using VFW in 2 types: `12x24px` / `24x24px`.
A regular western char has a width of `12 pixels` whilst most japanese chars `24 pixels`.

Regular text box holds a maximum of `3 text rows`.

`Each row` can be `480 px wide max`, after that next char will automatically `wrap` to the next row.


Other than ASCII, certain values provide additional text formatting / game global parameter / text effect, as per table below:

# Format

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






