# 1RENTA.bin TEXT STRUCT

Text stored in game executable is composed by `83 chunks` each one made by a `TEXT HEADER` and `TEXT DATA` part.

In order to call specific text, the game use one or multiple `TEXT DATA POINTERS` to specify the entry point of `TEXT DATA`within game executable. 


-`TEXT HEADER` : An array of `uint16` short values, representing each dialogue offset, starting from `TEXT DATA` multiplied by `0x2`.

-`TEXT DATA` : Game text using Rent a Hero Text Format.

-`TEXT POINTER OFFSET`: Data pointer specifying where to read `TEXT DATA`.



# CHUNK LIST:

|CHUNK NUMBER|TEXT DATA OFFSET|TEXT POINTER OFFSET|
|------------|-----------|------------|
|CHUNK  0|0x8c083658|0x8c04bd94|
|CHUNK  0|0x8c083666|0x8c04bd9c|
|CHUNK  0|0x8c083674|0x8c04bda0|
|CHUNK  1|0x8c0a717e|0x8c0161c0|
|    -   |     -    |0x8c0164f8|
|    -   |     -    |0x8c016768|
|    -   |     -    |0x8c0172b8|
|    -   |     -    |0x8c0175d8|
|CHUNK  2|0x8c0aad08|0x8c022470|
|    -   |     -    |0x8c0aad78|
|CHUNK  2|0x8c0aad0c|0x8c0aada4|
|    -   |     -    |0x8c0aadc8|
|    -   |     -    |0x8c0aadec|
|    -   |     -    |0x8c0aae40|
|CHUNK  2|0x8c0aad12|0x8c0aada0|
|    -   |     -    |0x8c0aadc4|
|    -   |     -    |0x8c0aade8|
|    -   |     -    |0x8c0aae08|
|CHUNK  2|0x8c0aad18|0x8c0aad7c|
|    -   |     -    |0x8c0aad54|
|    -   |     -    |0x8c0aad9c|
|    -   |     -    |0x8c0aadc0|
|    -   |     -    |0x8c0aade4|
|    -   |     -    |0x8c0aae04|
|    -   |     -    |0x8c0aae3c|
|    -   |     -    |0x8c0aae58|
|CHUNK  2|0x8c0aad1e|0x8c0aad58|
|    -   |     -    |0x8c0aad80|
|    -   |     -    |0x8c0aae5c|
|    -   |     -    |0x8c0aae20|
|CHUNK  2|0x8c0aad24|0x8c0aad5c|
|    -   |     -    |0x8c0aae24|
|CHUNK  2|0x8c0aad2a|0x8c022440|
|CHUNK  3|0x8c0d75da|0x8c049764|
|    -   |     -    |0x8c0498b8|
|    -   |     -    |0x8c04afc0|
|    -   |     -    |0x8c050ea8|
|    -   |     -    |0x8c05c0c0|
|    -   |     -    |0x8c05e14c|
|CHUNK  4|0x8c0d7d2c|0x8c04afb8|
|    -   |     -    |0x8c050eb0|
|    -   |     -    |0x8c05c0c8|
|    -   |     -    |0x8c05c6d8|
|CHUNK  5|0x8c0d968e|0x8c04f870|
|    -   |     -    |0x8c05cbd4|
|CHUNK  6|0x8c0db206|0x8c050f94|
|CHUNK  7|0x8c0dbcce|0x8c0495f4|
|    -   |     -    |0x8c05108c|
|    -   |     -    |0x8c05118c|
|    -   |     -    |0x8c05128c|
|CHUNK  8|0x8c0dbf12|0x8c051094|
|    -   |     -    |0x8c051194|
|    -   |     -    |0x8c051294|
|CHUNK  9|0x8c0dd2a8|0x8c048088|
|CHUNK 10|0x8c0dd31a|0x8c04acec|
|    -   |     -    |0x8c04b744|
|    -   |     -    |0x8c04bb1c|
|    -   |     -    |0x8c054438|
|CHUNK 11|0x8c0dd3cc|0x8c04b4f8|
|CHUNK 12|0x8c0dda0a|0x8c04de68|
|    -   |     -    |0x8c04f0ec|
|CHUNK 12|0x8c0ddb48|0x8c05b4dc|
|    -   |     -    |0x8c05b6e4|
|CHUNK 12|0x8c0ddb5e|0x8c046f28|
|    -   |     -    |0x8c05442c|
|CHUNK 12|0x8c0ddb74|0x8c055084|
|    -   |     -    |0x8c055548|
|CHUNK 12|0x8c0ddb78|0x8c05b4e8|
|    -   |     -    |0x8c05b6ec|
|CHUNK 12|0x8c0ddb80|0x8c05b4d4|
|CHUNK 12|0x8c0ddb84|0x8c05bb28|
|CHUNK 13|0x8c0ddbc2|0x8c04f248|
|CHUNK 14|0x8c0dddbe|0x8c057950|
|CHUNK 15|0x8c0de4ce|0x8c057948|
|CHUNK 16|0x8c0e158e|0x8c0175e8|
|    -   |     -    |0x8c058000|
|CHUNK 17|0x8c0e421e|0x8c04f9b4|
|CHUNK 18|0x8c0e4516|0x8c04f264|
|    -   |     -    |0x8c04fd24|
|CHUNK 19|0x8c0e45c2|0x8c04fd40|
|CHUNK 20|0x8c0e46bc|0x8c04f50c|
|    -   |     -    |0x8c05036c|
|    -   |     -    |0x8c050450|
|    -   |     -    |0x8c05380c|
|CHUNK 21|0x8c0e4826|0x8c053810|
|CHUNK 22|0x8c0e4d1a|0x8c0508fc|
|    -   |     -    |0x8c050a94|
|CHUNK 23|0x8c0e4d90|0x8c0508c8|
|    -   |     -    |0x8c050a9c|
|CHUNK 24|0x8c0e4e90|0x8c050904|
|    -   |     -    |0x8c050bb8|
|CHUNK 25|0x8c0e4efc|0x8c0508d0|
|    -   |     -    |0x8c050bc0|
|CHUNK 26|0x8c0e5006|0x8c05090c|
|    -   |     -    |0x8c050bd0|
|CHUNK 27|0x8c0e506c|0x8c0508d8|
|    -   |     -    |0x8c050bd8|
|CHUNK 28|0x8c0e5184|0x8c050914|
|    -   |     -    |0x8c050ce0|
|CHUNK 29|0x8c0e51f4|0x8c0508e0|
|    -   |     -    |0x8c050cf0|
|CHUNK 30|0x8c0e5450|0x8c0513cc|
|CHUNK 31|0x8c0e7a7e|0x8c050db8|
|CHUNK 32|0x8c0e9a42|0x8c0525a0|
|CHUNK 33|0x8c0ea00e|0x8c0526e4|
|CHUNK 34|0x8c0ea044|0x8c053554|
|CHUNK 35|0x8c0ea230|0x8c0537f4|
|CHUNK 36|0x8c0ea790|0x8c0540c4|
|CHUNK 37|0x8c0eaecc|0x8c055a1c|
|    -   |     -    |0x8c056940|
|CHUNK 38|0x8c0ebf1e|0x8c055a08|
|CHUNK 39|0x8c0ec1ec|0x8c057090|
|CHUNK 39|0x8c0ec228|0x8c05709c|
|CHUNK 40|0x8c0ec276|0x8c057968|
|CHUNK 41|0x8c0ec386|0x8c0581b8|
|CHUNK 42|0x8c0ec856|0x8c04f25c|
|    -   |     -    |0x8c058794|
|CHUNK 43|0x8c0ec9aa|0x8c058e44|
|    -   |     -    |0x8c059700|
|    -   |     -    |0x8c059a30|
|    -   |     -    |0x8c059b3c|
|CHUNK 44|0x8c0ecfa0|0x8c0594cc|
|    -   |     -    |0x8c0598d4|
|    -   |     -    |0x8c059a00|
|CHUNK 45|0x8c0ed2c0|0x8c05a790|
|    -   |     -    |0x8c05bb18|
|CHUNK 46|0x8c0ed59e|0x8c05a760|
|CHUNK 47|0x8c0ed5fe|0x8c05c0e0|
|    -   |     -    |0x8c05c688|
|CHUNK 48|0x8c0ed760|0x8c05cdac|
|CHUNK 49|0x8c0ed7c0|0x8c05d410|
|CHUNK 50|0x8c0f139e|0x8c06ab84|
|CHUNK 51|0x8c13fd96|0x8c14317c|
|    -   |     -    |0x8c1432f0|
|CHUNK 52|0x8c13feb0|0x8c143188|
|CHUNK 53|0x8c1400cc|0x8c143194|
|CHUNK 54|0x8c140276|0x8c1431a0|
|CHUNK 55|0x8c140426|0x8c1431ac|
|CHUNK 56|0x8c1405e0|0x8c1431b8|
|CHUNK 57|0x8c1406be|0x8c1431c4|
|CHUNK 58|0x8c14076a|0x8c1431d0|
|CHUNK 59|0x8c14081e|0x8c1431dc|
|CHUNK 60|0x8c140b1e|0x8c1431e8|
|CHUNK 61|0x8c141222|0x8c1431f4|
|CHUNK 62|0x8c14132c|0x8c143200|
|CHUNK 63|0x8c141492|0x8c14320c|
|CHUNK 64|0x8c141602|0x8c143218|
|CHUNK 65|0x8c14175a|0x8c143224|
|CHUNK 66|0x8c1419ee|0x8c143230|
|CHUNK 67|0x8c141c50|0x8c14323c|
|CHUNK 68|0x8c1420a0|0x8c143248|
|CHUNK 69|0x8c1421c2|0x8c143254|
|CHUNK 70|0x8c1422b0|0x8c143260|
|CHUNK 71|0x8c142444|0x8c14326c|
|CHUNK 72|0x8c1426aa|0x8c1432b4|
|CHUNK 73|0x8c1428d4|0x8c1432c0|
|CHUNK 74|0x8c1429f6|0x8c1432cc|
|CHUNK 75|0x8c142b1a|0x8c1432d8|
|CHUNK 76|0x8c142c5a|0x8c143278|
|CHUNK 77|0x8c142cae|0x8c143284|
|CHUNK 78|0x8c142d0a|0x8c143290|
|CHUNK 79|0x8c142d60|0x8c14329c|
|CHUNK 80|0x8c142db6|0x8c1432a8|
|CHUNK 81|0x8c142e24|0x8c1432e4|
|CHUNK 82|0x8c15d7c0|0x8c07aca8|
|CHUNK 83|0x8c15d91e|0x8c07ade0|

