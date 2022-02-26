### String 

`endsWith()` : method

___

#### Description and Return Value:

The `endsWith()` method checks if its argument includes the last character in its *calling string*. Returns `true` if it is included, `false` if not. 

It has an optional **second argument** that represents the index value **after** the last character's index in the *calling string*. If this second argument is not provided, it defaults to the length of the string `str.length`. This represents where to stop the search.

Method is `case-sensitive`


`str.endsWith('.')`
`str.endsWith('lastfewchars', 10)`
___

#### Parameters

1. `characters` to be searched for at the end of the calling string

<br>

2. `optional length` (integer) that indicates the end of search, character at this index is not included. Defaults to the array length if omitted.

```
callStr.endsWith(characters);
callStr.endsWith(characters, length);
```
___

#### Example:

```
let str = 'Cats are the best!';

console.log(str.endsWith('best'));  //false
console.log(str.endsWith('st!'));   //true
console.log(str.endsWith('Ca', 2)); //true
```
last character is `!` in the calling string