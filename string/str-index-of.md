### String 

`indexOf()` : method

___

#### Description and Return Value:

The `indexOf()` method searches its calling string for the specified string in its argument. If found, it returns the `index` of the **first** occurence of the string to be found. If it is a word with more than one character, the index of its `first character` is returned. 

If string is not found, the return value is `-1`


`strCaller.includes(strFind);`

`includes()` is **case sensitive**

___

#### Parameters

1. `string` value to be searched within the method's string caller.

2. Optional `position` parameter that indicates what index to **begin** searching for the `string` value in its argument. 

    <br>

    - If `position >= length of the calling string`, method doesn't search the calling string at all-- will `return -1`
    
    <br>

    - If `position < 0`, method will default position to `0`.



`strCaller.includes(strFind);`

`strCaller.includes(strFind, position);`

___

#### Example:

```
let sentence = 'No better time than the present.';

let word = 'present';

console.log(sentence.length);                 // 32
console.log(sentence.indexOf('present', 47)); // -1
console.log(sentence.indexOf('present'));     // 24

```
If the `position` indicated (representing the `index`) surpasses the location of the existing string, method will return `-1`.

The `index` of the `first character` in the `first occurence` of the string argument in the calling string is returned.
