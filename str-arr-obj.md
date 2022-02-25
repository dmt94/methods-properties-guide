### Everything is covered here

##### Ultimate Cheatsheet

`String` 


`Array` 


`Object`
___

#### `String` Properties and Methods

| Name       | Description   | Parameters | Errors/Unexpected  | Return Value  |
| ----       | -----------   | ---------- | ------------ | ------------ |
| `.length`   | represents the length of the string, <br> including whitespace characters | N/A | - escape sequences have `1` length | - returns the `length` of its string caller <br> - returns undefined for non-string values <br> - returns `0` for an empty string | <!--- End -->
| `.charAt()`   | searches its string caller for the character<br> with the index value given in its argument | 1. integer from `0` to `string.length - 1` <br><br> - Default to `0` if no parameter  | ------------ | returns the `character` with the matching index value in its argument | <!--- End -->
| `.concat()`    | concatenates the strings in its argument to its string caller   | - Multiple allowed separated by a comma <br> `str.concat(' ', 'str')` <br> - No parameters returns string caller | non-string arguments are converted to strings | a `new string` that starts with its string caller followed by its arguments | <!--- End -->
| ----       | -----------   | ---------- | ------------ | ------------ |


