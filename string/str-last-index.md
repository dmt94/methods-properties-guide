### String 

`lastIndexOf()` : method

___

#### Description and Return Value:

`lastIndexOf()` searches its string caller for the string in its argument, and returns the index of its **last occurence**

`lastIndexOf(searchString)`
`lastIndexOf(searchString, position)`

##### Return Value

`index` of the last occurence of its argument string
`-1` if argument string is not found
___

#### Parameters

1. `searchString`
- `string` to search for in the method's calling string

    <br>

    - IF `no arguments` given, `searchString` defaults to `undefined`, which gets **coerced** into the string `"undefined"`
    ```
    console.log("It is undefined".lastIndexOf()); // 6 
    ```

2. `OPTIONAL: position`
- `integer` that specifies the `index` to end the search for the `searchString` in its argument.

    <br>

    - IF `position` is specified at an index before an existing `searchString`, then `returns -1`
    ```
    let word = 'hi universe hi';

    console.log(word.lastIndexOf('universe', 1)); // -1
    ```

    <br>

    - IF `position > length of calling string`, method searches entire string

    ```
    let word = 'hi universe hi';

    console.log(word.lastIndexOf('hi', 100));  // 12
    ```

    <br>

    - IF `position <= 0`, method will only search at `index 0` and confirm if the argument string is found there

    ```
    let word = 'Joyous JavaScript';

    console.log(word.lastIndexOf('Java', -2)); // -1
    console.log(word.lastIndexOf('Joy', 20));  // 0
    ```
___

#### Example:

```
let word = 'Joyous JavaScript';

console.log(word.lastIndexOf('Scr', 35));          // 11
console.log(word.lastIndexOf(undefined));          // -1 (undefined -> 'undefined')
console.log(word.lastIndexOf());                   // -1 (empty = undefined -> 'undefined')
console.log(word.lastIndexOf('J', undefined));     // 7 (position defaults to length of string)

console.log(word.lastIndexOf(''));                 // 17 = length of string 
console.log(word.lastIndexOf('', 2));              // 2
console.log(word.lastIndexOf('', 9));              // 9 
```
- `empty string` as an argument returns the `length` of string caller

<br>

- `empty string` with a position argument returns the `position`

