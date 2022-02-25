### String 

`replaceAll()` : method

___

#### Description and Return Value:

The `replaceAll()` method searches for the **pattern** (can be `string` or `RegExp`) indicated in its first argument on its calling string. 

If found, it returns a new string that **replaced all** the **pattern** found indicated with the `string` or `function that can be invoked for each match` in its second argument.


`strCaller.replaceAll(pattern, replacement);`
`strCaller.replaceAll(pattern, replacerFunction);`

___

#### Parameters

1. `Pattern`
- RegExp object or literal
- String

2. `Replacement`
- String (replaces the RegExp or String parameter)
- Function 

___

#### Example:

```
let statement = "produce at an elite level. Very elite.";

console.log(statement.replaceAll('elite', 'extraordinary'));

// 'produce at an extraordinary level. Very extraordinary.'
```


