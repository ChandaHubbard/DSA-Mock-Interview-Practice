### numberOfPalindromes

Given a string, write an algorithm to count the number of words in the string that are palindromes. The output must include a list of the palindromes and the number of palindromes.

   - Input: `"Dad gave mom a Tesla as a racecar"`
   - Output: `Dad, mom, racecar, 3 Palindromes`
   
 ## My Solution
 
 ````
function howManyPalindromes(str) {
let whichOnesAndHowMany = str.split(" ").filter(x => 
   x.toLowerCase() === x.toLowerCase().split("").reverse().join("")
   && x.length > 1)
return `${whichOnesAndHowMany.join(", ")}, ${whichOnesAndHowMany.length} Palindromes`
}
````
### Input

```
let sentence = "Dad gave mom a Tesla as a racecar"
```

### Output

```
'Dad, mom, racecar, 3 Palindromes'
```
 
 ## Optimal Solution as Algorithm
