### String 

`startsWith()` : method

___

#### Description and Return Value:

`startsWith()` determines whether a string begins with the characters specified in its argument, returning the appropriate boolean values `true` or `false`.

`startsWith(searchString)`
`startsWith(searchString, position)`

##### Return Value

`true` if given strings are found and `false` if not.
___

#### Parameters

1. `searchString`
- characters to be searched for at the start of the string


2. `OPTIONAL: position`
- indicates the index value to begin searching for `searchString`. Defaults to `0`, if omitted.

___

#### Example:

```
let hanhQuote = 'Letting go gives us freedom';

console.log(hanhQuote.startsWith())        // false
console.log(hanhQuote.startsWith('L'))     // true
console.log(hanhQuote.startsWith('Let'))   // true
console.log(hanhQuote.startsWith(' ', 7))  // true
console.log(hanhQuote.startsWith('go', 8)) // true
```

