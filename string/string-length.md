### String 

`length` : property

___

#### Also a property of:

`Array`

---

#### Description and Return Value:

The `length` property of a string will return a number that represents the length of the string, including whitespace characters. The `length` property will always return one number higher than the final index of the string.

The return value of an empty string is `0`

```
let emptyStr = '';
console.log(emptyStr);  // 0
```

___

#### Example:

```
let strOne = 'orange';
let strWithNewline = 'orange\n";
let strTwo = 'stay present';
let emptyStr = '';
let spaceStr = ' ';
let newlineStr = '\n';


console.log(strOne.length);         // 6
console.log(strWithNewLine.length); // 7
console.log(strTwo.length);         // 12
console.log(emptyStr.length);       // 0
console.log(spaceStr.length);       // 1
console.log(newlineStr.length);     // 1

```

___

#### Possible Uses:

Finding the last index of a string:

```

let string = 'learning';
let lastIndex = string.length - 1;

console.log(string.length) // 8
console.log(lastIndex);    // 7
console.log(string[7]);    // 'g'

```