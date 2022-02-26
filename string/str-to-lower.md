### String 

`toLowerCase()` : method

___

#### Description and Return Value:

`toLowerCase()` returns a new string that is a copy of its calling string in an all **lowercase** format.

##### Return Value

`new string` that represents the calling string in all lowercase.

`'CALLINGSTRING'.toLowerCase()` >> `'callingstring'`
___

#### Parameters

`NO PARAMETERS`
___

#### Example:

```
console.log('TODAY'.toLowerCase());           // 'today'
console.log('TODAY'.toLowerCase(3));          // 'today'
console.log('TODAY'.toLowerCase('tomorrow')); // 'today'
console.log('TODAY'.toLowerCase(null));       // 'today'
console.log('TODAY'.toLowerCase(undefined));  // 'today'
console.log('TODAY'.toLowerCase(NaN));        // 'today'
```

