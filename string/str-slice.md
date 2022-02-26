### String 

`slice()` : method

___

#### Description and Return Value:

`slice()` takes a part of its string caller and returns a new string with a copy of this extraction, depending on the index portion indicated in its argument.

`strCaller.slice(beginIndex);`
`strCaller.slice(beginIndex, endIndex);`

___

#### Parameters

1. `beginIndex`
- Zero-based index , where extraction is set to begin

    - IF `beginIndex is negative`: extraction begins at `strCaller.length + beginIndex`
      - `"test".slice(-2)` >> `st`
      - 4 + (-2) = 2 (index 2 = s)
      - count backwards
    
    - IF `beginIndex >= str.length`: `empty string` is returned `""`

2. `OPTIONAL: endIndex`
- indicates where to end extraction, character at this index is `not included`.

    - IF endIndex is `omitted`, `undefined`, `greater than length of string` or can't be converted into a number, endIndex defaults to length of string, it extracts to the end of the string.
   
    - count backwards if `negative` and don't include character

___

#### Example:

```
let word = 'gainful';


console.log(word.slice(-1))           // 'l'
console.log(word.slice(2, 4))         // 'in
console.log(word.slice(1, undefined)) // 'ful'
console.log('lily'.slice(1));         // 'ily'

let newWord = word.slice(4, undefined);

console.log('plenti'.concat(newWord)); // `plentiful`

```

