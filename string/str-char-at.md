### String 

`chatAt()` : method

___

#### Description and Return Value:

The `charAt()` method will return the character at the specified index in its argument:

`str.charAt(index)`

If the index indicated in its argument is out of range, then it will return an `empty string`

If **no** index is indicated, the default index will be `0`

```
let str = 'apple';

console.log(str2.charAt(15)); // '' >> argument out of range

console.log(str2.charAt());   // 'a' >> no index indicated
```

___

#### Parameters

`index` value, between `0` and `length of string - 1`:
>`Range: 0 to (str.length - 1)`
___

#### Example:

```
let str = 'plum village';

console.log(str.charAt(2));               // 'u'
console.log(str.charAt(str.length - 1));  // 'e'
console.log(str.charAt(15));              // ''

```

___

#### Possible Uses:

Check if the first character in a string is capitalized

```

let str = 'universe';

console.log(str.charAt(0) === str[0].toUpperCase() ? true : false) // false

```