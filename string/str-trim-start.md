### String 

`trimStart()` or `trimLeft()`: method

___

#### Description and Return Value:

`trimStart()` ***removes*** any existing **whitespace** characters (space, tab, etc.) and all **line terminator** characters (command returns `(\r`), line feed `(\n)`, etc.) located at the **start** of its string caller, returning a `new string` without these characters.

`caller.trimStart()`
<br>
##### Return Value

`new string` value representing its calling string, without any existing whitespace from the beginning.

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

console.log(space.trimStart()); // empty string ''
console.log(space2.trimStart()); // 'ok  '
console.log(space3.trimStart()); // 'o k  ';
```

