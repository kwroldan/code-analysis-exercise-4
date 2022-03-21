# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

*SUMMARY* 
1) The function converts the number entered into an array of string values, splitting each individual character of the string.
2) The function then reverses the array created from step 1.
3) A new blank array is created.
4) Using the `for...of` loop, it takes the reversed array created in step 2 and converts each item to number values from string values, and adds it to the blank array created in Step 3.
5) The new array is returned at the end of the function.

```js
function (number){
  let numberArray = `${number}`.split("")
  let reversedNumberArray = numberArray.reverse()

  let newArray = []
  for (number of reversedNumberArray){
    newArray.push(+number)
  }

  return newArray
}
```

| Input | Output      |
| ----- | ----------- |
| 1234  | [4, 3, 2, 1]|
| 56    | [6, 5]      | 
| 0     | [0]         | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>The program reverses the number you created and returns it in an array of number values.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
