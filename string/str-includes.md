### String 

`includes()` : method

___

#### Description and Return Value:

The `includes()` method returns `true` or `false` depending on whether the string in its argument is included in its string caller. 


`strCaller.includes(strFind);`

`includes()` is **case sensitive**

___

#### Parameters

1. `string` value to be searched within the method's string caller.

2. Optional `position` parameter that indicates what index to **begin** searching for the `string` value in its argument.


`strCaller.includes(strFind);`

`strCaller.includes(strFind, position);`

___

#### Example:

```
let sentence = 'The quick brown fox jumps over the lazy dog.';

let word = 'fox';

console.log(sentence.includes('fox'))     //true 
console.log(sentence.includes('fox', 5))  //true 
console.log(sentence.includes('fox', 20)) //false
```
If the position indicated (representing the `index`) surpasses the location of the existing string, method will return `false`
