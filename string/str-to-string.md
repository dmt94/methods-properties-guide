### String 

`toString()` : method

___

#### Description and Return Value:

`toString()` is typically used when an object needs to be displayed as a text, or when an object needs to be used as a string. Returns the value of a String object as a `string`. This method can also coerce a `number` into a `string`.

##### Return Value

`string` value of its caller

`caller.toString()`
___

#### Parameters

`NO PARAMETERS`
___

#### Example:

```

let num = 1;
let nanV = NaN;
let nullV = null;
let undef = undefined;

console.log(num.toString());         // '1'
console.log(nanV.toString());        // 'NaN' (a numerical result, can be converted to string)
console.log(nullV.toString());       // TypeError: Cannot read properties of null
console.log(undef.toString());       // TypeError: Cannot read properties of undefined



let retNum = function() {
  return 23;
}

console.log(retNum);                  
/* function() {      function is coerced into a literal string without invocation
  return 23;
}
*/

console.log(retNum().toString());  // '23', with function invocation


let phrase = new String('mindful breathing');   // String object is created

console.log(phrase.toString());                 // 'mindful breathing'
```

