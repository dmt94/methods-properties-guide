### Everything is covered here

##### Ultimate Cheatsheet

`String` 


`Array` 


`Object`
___

#### `String` Properties and Methods

| Name       | Description   | Parameters | Errors/Unexpected  | Return Value  |
| ----       | -----------   | ---------- | ------------ | ------------ |
| `.length`   | represents the length of the string, <br> including whitespace characters | N/A | escape sequences have `1` length | - returns the `length` of its string caller <br> - returns undefined for non-string values <br> - returns `0` for an empty string | <!--- End -->
| `.charAt()`   | searches its string caller for the character<br> with the index value given in its argument | 1. integer from `0` to `string.length - 1` <br><br> - Default to `0` if no parameter <br><br> `red.charAt(1);` | ------------ | returns the `character` with the matching index value in its argument | <!--- End -->
| `.concat()`    | concatenates the strings in its argument to its string caller   | - Multiple allowed separated by a comma <br> `str.concat(' ', 'str3');` <br><br> - No parameters returns string caller | non-string arguments are converted to strings | a `new string` that starts with its string caller followed by its arguments | <!--- End -->
| `.endsWith()`       | checks if its argument includes the last character in its calling string  | 1. A string, to be searched for at the end of the calling string <br><br> 2. `optional length` (integer) to represent index value to end search. Defaults to `array length` if omited <br><br> `str.endsWith('tail', 3);` | ------------ | Returns boolean values `true` or `false` |
| `.charCodeAt()`       | searches for the `character` in its string caller that matches the `index` given in its argument and returns its corresponding `UTF-16 code unit`   | 1. integer from `0` to `string.length - 1` <br><br> - If given index is less than 0 or greater than the string caller's last available index, `returns NaN` <br><br> - string values and `no parameter` defaults to `0` | index that is out of range returns `NaN` | returns the `UTF-16 code unit` of the character whose index value matches its argument | <!--- End -->
| `String.fromCharCode()`   | will return the string associated with the UTF-16 code units given in its argument   | 1. `Multiple possible` UTF-16 code units ranging from `0 to 65535`, separated by a comma <br><br> - If argument is `omited `or a `string`, method returns an `empty string` <br><br> `String.fromCharCode(79, 75);` | ------------ | returns a `string` created from the given sequence of `UTF-16` code units in its argument | <!--- End -->
| `String.fromCodePoint()`  | returns a string created from the given sequence of code points in its argument  | 1. `Multiple possible` numbers that represent `code points` <br><br> `String.fromCharCode(55356, 57091)`; | `invalid Unicode code point` argument will throw a `RangeError` | returns `string` created from the given sequence in its argument | <!--- End -->
| `.includes()`  | searches if its string caller includes the string in its argument | 1. `string` value to be searched within the string caller <br><br> 2. `optional position`, represents index to **begin** the search for the argument string within the string caller <br><br> `strCaller.includes(strFind, position);` | If the position indicated for its second argument **surpasses the location** of the string caller, will return `false` | returns boolean values `true` or `false` | <!--- End -->
| `.indexOf()`   | searches its calling string for the specified string in its argument, returning the index of its first occurence.   | 1. `string` to be searched within the string caller <br><br> 2. `optional position` represents index to **begin** the search for the `string` value on the string caller <br><br> `strCaller.indexOf(strFind, position);` | If `position` is >= length of calling string, `returns -1` <br><br> If `position` is less than 0, `default position = 0` | returns `index` of the first occurence of the string to be found. If it is a word with more than one character, the index of its `first character` is returned. <br><br> If string is not found, `returns -1` | <!--- End -->
| `.repeat()`    | creates and returns a copy of its calling string, concatenated together with other copies depending on the `amount` indicated in its argument | 1. `integer` between 0 - Infinity, indicating the number of times to repeat the string <br><br> `'hello'.repeat(3);` | - `argument < 0`: `RangeError` is thrown <br><br> - `argument = 0`: `empty string ''` is returned <br><br> - `argument = decimal`: decimal rounds down to integer | `new string` copy of its calling string concatenated with other copies | <!--- End -->
| `.replace()`   | searches for the pattern given in argument on its calling string and if found, replaces first found pattern with the replacement `string` or `function` given in argument  | 1. `pattern` that can be a `RegExp object or literal` or `String` <br><br> 2. `replacement` can be a `String` or `Function` <br><br> `str.replace('cat', 'dog);` |  | returns `new string` with some or all matches of a pattern replaced by indicated replacement | <!--- End -->
| `.replaceAll()` | searches for the pattern given in argument on its calling string and if found, replaces all found pattern with the replacement `string` or `function` given in argument   | 1. `pattern` that can be a `RegExp object or literal` or `String` <br><br> 2. `replacement` can be a `String` or `Function` <br><br> `str.replaceAll(/b/g, 'B')` <br><br> when using `regex` to search, must be `global` | ------------ | `new string` with `all` matches of a pattern replaced by replacement argument |
| ----       | -----------   | ---------- | ------------ | ------------ |