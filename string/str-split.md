### String 

`split()` : method

___

#### Description and Return Value:

`split()` takes apart its string caller, dividing them into substrings, depending on the separator indicated in its argument. The `return` value is an array with each substring as an element.

`strCaller.split('');`  splits into its UTF-16 "characters" 
`strCaller.split(' ');` 

##### Return Value

`Array` of strings, split at each point where its `separator` argument occurs in its string caller.
___

#### Parameters

1. `separator`
- indicates where each split should occur.

    - `String`
      - IF separator is `omitted` or `does not occur` in calling string, the returned array is the calling string as one element

        - `['okay]`
    <br>
      - IF separator is found at the `beginning` or `end` of the calling string, a split will still occur, but an empty string will appear at its beginning or ending position

        - `[ '', 'peace', 'is', 'already', 'yours', '' ]`
    <br>
     - IF separator is an empty string (''), the calling string is converted to an array of each of its UTF-16 "characters"
    
        - `'red'.split('')` >> `['r', 'e', 'd']`
    <br>
    - `RegExp`



2. `OPTIONAL: limit`
- non-negative integer that specifies a limit on the number of substrings to be included in the array. If provided, string is split at each occurence of its separator argument, but stops when `limit entries` have been placed in the array.

    - IF limit is `0`, `[]` is returned
    `'move on'.split(' ', 0)` >> `[]`
    <br>
    - if there are less entries than the limit given, then all the possible entries will still be returned

___

#### Example:

```
let hanhQuote = 'Life is available only in the present';


let hanhArr = hanhQuote.split(' ');

console.log(hanhArr);         // [ 'Life', 'is', 'available', 'only', 'in', 'the', 'present' ]

console.log('joy'.split('')); // ['j', 'o', 'y']
```

