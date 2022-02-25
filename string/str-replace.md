### String 

`replace()` : method

___

#### Description and Return Value:

The `replace()` method searches for the **pattern** (can be `string` or `RegExp`) indicated in its first argument on its calling string. 

If found, it returns a new string that **replaced** the **pattern** indicated with the `string` or `function that can be invoked for each match` in its second argument.

If the **pattern** is a `string`, only the first occurence found will be replaced.

`strCaller.replace(pattern, replacement);`
`strCaller.replace(pattern, replacerFunction);`

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

console.log(statement.replace('elite', 'extraordinary'));

// 'produce at an extraordinary level. Very elite.'
```

