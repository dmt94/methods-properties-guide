### String 

`trim()` : method

___

#### Description and Return Value:

`trim()` ***removes*** any existing **whitespace** characters (space, tab, etc.) and all **line terminator** characters (command returns `(\r`), line feed `(\n)`, etc.) located at the beginning **and** end of its string caller, returning a `new string` without these characters.

`caller.trim()`
<br>
##### Return Value

`new string` value representing its calling string, without any existing whitespace from either sides. 

if `no whitespace` exists, a copy of its calling string is returned essentially.

___

#### Parameters

`NO PARAMETERS`
___

#### Example:

```
let space = '   ';
let space2 = '  ok  ';
let space3 = '  o k  ';

let afterSpace = space.trim();

console.log(space.trim());        // empty string ''
console.log(afterSpace.length);   // 0 
console.log(space2.trim());       // 'ok'
console.log(space3.trim());       // 'o k'  
```

