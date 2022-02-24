### String 

`concat()` : method

___

#### Description and Return Value:

The `concat()` method returns a new string, the result of concatenating the string(s) in its argument to the calling string.

`firstStr.charCodeAt(secStr, thirdStr, ...nStr);`



If its argument contains a **non-string type**, it will convert the non-string type to a string value before concatenating.



```
console.log('Good'.concat(' ', 'Afternoon'));   // Good Afternoon
console.log('Good'.concat(' ', null));          // Good null
console.log('Good'.concat(' ', undefined));     // Good undefined
console.log('Good'.concat(' ', NaN));           // Good NaN
console.log('Good'.concat(' ', 22));            // Good 22
```

___

#### Parameters

One ore more `string` values

```
firstStr.charCodeAt(secStr, thirdStr, ...nStr);
```
___

#### Example:

```
let str = 'Nice';

console.log(str.concat(' ', 'Day'));   // 'Nice Day'
console.log(str.concat(' ', 'Night')); // 'Nice Night'
```

___

#### Alternative:

Using the `+=` or `+` to concatenate strings

```
let str = 'first';

let str2 = 'second';

let str3 = 'third';

let finalStr = str + ' ' + str2 + ' ' + str3;

console.log(finalStr); // 'first second third'
```

```
let glue = ''

let arr = ['w', 'i', 's', 'd', 'o', 'm'];

arr.forEach(char => glue += char);

console.log(glue);   // 'wisdom'
```