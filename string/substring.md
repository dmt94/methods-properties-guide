### String 

`substring()` : method

___

#### Description and Return Value:

`substring()` extracts a part of its string caller and returns a new string that contains the extracted substring, depending on the index values indicated in its argument.

`substring(indexStart)`
`substring(indexStart, indexEnd)`

##### Return Value

`new string` containing the specified part of the calling string
___

#### Parameters

1. `indexStart`
- index of the first character to **include** in the returned substring

    <br>

    - IF `indexStart < 0`, indexStart defaults to `0`
    ```
    let word = 'sparking probiotic';

    console.log(word.substring(-1)); // 'sparkling probiotic'
    ```

    <br>

    - IF `indexStart > calling string length`, indexStarts defaults to `string.length` returns `empty string`
    ```
    let word = 'sparking probiotic'; 

    console.log(word.length); // 18
    console.log(word.substring(19)); // ''
    ```


2. `OPTIONAL: indexEnd`
- index of the first character to **exclude** from the returned substring

    <br>

    - IF `indexEnd` is omitted, method extracts characters to the end of the string :
    ```
    let word = 'sparking probiotic';

    console.log(word.substring()); // 'sparkling probiotic'
    ```

    <br>

    - IF `indexStart = indexEnd`, method returns an `empty string ''` :

    ```
    let word = 'sparking probiotic';

    console.log(word.substring(4,4)); // ''
    ```

    <br>

    - IF `indexStart > indexEnd`, method will return a string where it appears as if its argument values are 'swapped' : 

    ```
    let word = 'sparking probiotic';

    console.log(word.substring(15, 3)); // 'rking probio'
    ```

If `no` arguments are given, method returns a `new string` that is a copy of its `string caller`

___

#### Example:

```

let word = 'determined';

console.log(word.substring(2, 5));         // 'ter'
console.log(word.substring(5, 9));         // 'mine'
console.log(word.substring(0));            // 'determined'
console.log(word.substring());             // 'determined'
console.log(word.substring(-1));           // 'determined'
console.log(word.substring(20));           // ''
console.log(word.substring(2, 2));         // ''

console.log(word.substring(6, 2));         // 'term' (indexStart and indexEnd swap)

console.log(word.substring(0, undefined));          // 'determined' (undefined is same as omitted)
console.log(word.substring(undefined, undefined));  // 'determined' (same as no argument)
console.log(word.substring(undefined, 5));          // 'deter' 
```
`undefined` for `firstIndex` defaults to `0`
`undefined` for `indexEmd` defaults to `string.length`


