# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (number){                                    //34
  let numberArray = `${number}`.split("")             // ["3","4"]
  let reversedNumberArray = numberArray.reverse()     // ["4", "3"]

  let newArray = []                                     
  for (number in reversedNumberArray){                // 0
    newArray.push(+number)                            // newArray == {0} -> [0,1]
  }

  return newArray
}
```

| Input | Output |
| ----- | ------ |
|   34    |    [0,1]    | 
|   52    |    [0,1]    | 
|   630   |    [0,1,2]    | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>
    This program takes a given number, turns it into a string, then splits it forming an array comprised of the individual digits that 
    first comprised the number. That array is then reversed to form the final reversedNumberArray. Then, the program creates a newArray out of 
    the indexes of the old array, starting at 0 and ending at the last array position number the reversedNumberArray had. In this process, 
    the function also changes the digits back to numbers.
    </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
