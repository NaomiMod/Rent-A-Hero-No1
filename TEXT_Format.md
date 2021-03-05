#  Text format struct

Every char is mapped by a `uint16` short value, corresponding to a ASCII character used by game font.

Regular text box holds a maximum of `3 text rows`.

`Each row` can be `320 px wide max`, after that it will automatically `cut & wrap text` to the next row.

A regular western char is usually taking `8 pixels` whilst most of japanese chars `16 pixels`.

Other than ASCII, certain values provide additional text formatting / game global parameter / text effect, as per table below:

# Format

|Value|Description|
|-------|------------|
|0x0180|  Return, next row|
|0x0280|  Clear all text *|
|0xa74d|	SPACE (8px)|
|0x504e|	SPACE (8px)|
|0x0000|  SPACE (16px)|
|0x0080|  End of sequence|

# Special Effects & Global Values

|Value|Description|
|-------|------------|
|0x0097|  Effect: Shake Text Box|
|0x0190|  HERO FIRST NAME|
|0x0290|  HERO LAST NAME|
|0x0390|  HERO FIRST NAME|
|0x0490|  HERO LAST NAME|
|0x0590|  UNK_GLOBAL_VALUE|
|0x0690|  UNK_GLOBAL_VALUE2|
|0x1088|  MONEY|
|0x10a0|  ENERGY DRINK|
|0x5088|  BATTLES WON|
|0x5188|  BATTLES LOST|


*Used to display long text continuously,.







