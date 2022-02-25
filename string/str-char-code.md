### String 

`charCodeAt()` : method

___

#### Description and Return Value:

The `chatCodeAt()` method will return an integer between `0` and `65535`, which represents the unique `UTF-16 code unit` of the character that matches the index given in its argument.

`str.charCodeAt(index);`

If the index given is out of range, `charCodeAt()` will return `NaN`:

>if given index < 0 || index >= str.length

```
console.log('ABC'.charCodeAt(-1));    // NaN

console.log('ABC'.charCodeAt(5));     // NaN

console.log('ABC'.charCodeAt('abc')); // 65 , argument defaults to 0

console.log('ABC'.charCodeAt(0));     // 65 

```
The character `A` corresponds to UTF-16 code `65`

___

#### Parameters

`index` value, between `0` and `length of string - 1`:
>`Range: 0 to (str.length - 1)`

If `index` value is not a number, it defaults to `0`
___

#### Example:

```
let str = 'language';

console.log(str.charCodeAt(4)); // 117
```
The character `u` corresponds to UTF-16 code `117`
