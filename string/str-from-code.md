### String 

`String.fromCodePoint()` : method

___

#### Description and Return Value:

The `String.fromCodePoint()` **static** method returns a **string** created from the given sequence of code points in its argument.
___

#### Parameters

Any sequence of numbers that represent code points (separated by a comma `,` if more than one argument supplied).

If **invalid** `Unicode code point` is given, then a `RangeError` is thrown:

```
String.fromCodePoint('_');      // RangeError
String.fromCodePoint(Infinity); // RangeError
String.fromCodePoint(-1);       // RangeError
String.fromCodePoint(3.14);     // RangeError
String.fromCodePoint(3e-2);     // RangeError
String.fromCodePoint(NaN);      // RangeError
```
___

#### Example:

```
console.log(String.fromCodePoint(42));       // "*"
console.log(String.fromCodePoint(67, 65));   // "CA"
console.log(String.fromCodePoint(0x1F31E));  //  🌞
console.log(String.fromCodePoint(0x1F31C));  //  🌜
```

___

#### Alternative:

[`String.fromCharCode()`](/string/str-from-char.md)
<br>

***(MDN Definition)***

**String.fromCharCode( )** :

**cannot** `return` supplementary characters (code points 0x010000 - 0x10FFFF) by specifying their **code points**. It requires the UTF-16 surrogate pair in order to return a supplementary character.

```
console.log(String.fromCharCode(55356, 57091));    // 🌃
console.log(String.fromCharCode(0xD83C, 0xDF03));  // 🌃
```

**String.fromCodePoint()** :

**can** `return` 4-byte supplementary characters, as well as 2-byte BMP characters, by specifying their `code point`, which is equivalent to the `UTF-32 code unit`

```
console.log(String.fromCodePoint(0x1F338));       // 🌸
```


