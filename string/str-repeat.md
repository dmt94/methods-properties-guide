### String 

`repeat()` : method

___

#### Description and Return Value:

The `repeat()` method creates and returns a new string that looks like a copy of its string caller, concatenated together with other copies of it. The amount of copies produced is indicated by its argument. 

`strCaller.repeat(number);`

___

#### Parameters

`Integer`, between `0` to `Infinity`, indicating the number of times to repeat the string

- If `argument < 0` , a `RangeError` is thrown
- If `argument = 0` , An empty string is returned `''`
- If `argument = decimal` , Decimal is converted into Integer, rounding down:

```
console.log('abc'.repeat(3.2)) // 'abcabcabc'
```

___

#### Example:

```
console.log('copycat '.repeat(3)) // 'copycat copycat copycat'

console.log('💜'.repeat(3));      //  '💜💜💜'

```

