### String 

`String.fromCharCode()` : method

___

#### Description and Return Value:

The `String.fromCharCode()` **static** method returns a **string** created from the given sequence of UTF-16 code units in its argument.


`String.fromCharCode(65)` returns `A`
`String.fromCharCode(65, 66)` returns `AB`
___

#### Parameters

Any sequence of numbers that represent UTF-16 code units (separated by a comma `,` if more than one argument supplied) ranging from `0` to `65535`.  

If **no** argument is given or a **string** argument is given, method returns an `empty string`
___

#### Example:

```
console.log(String.fromCharCode(9829));    // ♥
console.log(String.fromCharCode(79, 75));  // OK
console.log(String.fromCharCode(73, 32, 9829, 32, 74, 83));  // I ♥ JS
console.log(String.fromCharCode(0xD83C, 0xDF03)); // 🌃
```

___

#### Alternative:


***(MDN Definition)***


[`String.fromCodePoint()`](/string/str-from-code.md)

**can** `return` 4-byte supplementary characters, as well as 2-byte BMP characters, by specifying their `code point`, which is equivalent to the `UTF-32 code unit`

```
console.log(String.fromCodePoint(0x1F338));       // 🌸
```

**String.fromCharCode( )** :

**cannot** `return` supplementary characters (code points 0x010000 - 0x10FFFF) by specifying their **code points**. It requires the UTF-16 surrogate pair in order to return a supplementary character.

```
console.log(String.fromCharCode(55356, 57091));    // 🌃
console.log(String.fromCharCode(0xD83C, 0xDF03));  // 🌃
```


