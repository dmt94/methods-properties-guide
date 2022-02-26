### String 

`trimEnd()` or `trimRight()` : method

___

#### Description and Return Value:

`trim()` ***removes*** any existing **whitespace** characters (space, tab, etc.) and all **line terminator** characters (command returns `(\r`), line feed `(\n)`, etc.) located at the **end** of its string caller, returning a `new string` without these characters.

`caller.trimEnd()`
<br>
##### Return Value

`new string` value representing its calling string, without any existing whitespace after it. 

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

console.log(space.trimEnd()); // empty string ''
console.log(space2.trimEnd()); // '  ok'
console.log(space3.trimEnd()); // '  o k';


let sentence = 'to be ever present is a present\n';

console.log(sentence);
/* 'to be ever present is a present

'
*/

console.log(sentence.trimEnd()); // 'to be ever present is a present'
```

