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


2. `OPTIONAL: indexEnd`
- index of the first character to **exclude** from the returned substring

    - IF `indexEnd` is omitted, method extracts characters to the end of the string
    <br>
    - IF `indexStart = indexEnd`, method returns an `empty string ''`
    <br>
    - IF `indexStart > indexEnd`, method will return a string where it appears as if its argument values are 'swapped': 

    ```
    let word = 'sparking probiotic';

    console.log(word.substring(15, 3)); // 'rking probio'
    ```

If `no` arguments are given, method returns a new string that is a copy of its `string caller`

**Argument values:**

`argument < 0` defaults to `0`
`argument > string.length` defaults to `string.length`
___

#### Example:

```

```

