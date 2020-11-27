# Word Occurances

Given a document, implement an algorithm to count the number of word occurrences.

### Input: 
`let sentence = "Hello there, how are you? Can you tell me how to get to the nearest Starbucks?"`

### Output: 
````
{
  Hello: 1,
  there: 1,
  how: 2,
  are: 1,
  you: 2,
  Can: 1,
  tell: 1,
  me: 1,
  to: 2,
  get: 1,
  the: 1,
  nearest: 1,
  Starbucks: 1
}
````


## My Solution 

````
const findOcc = (words) => {
let freq = {}
words = words.replace(/[^\w\s]/g, "")
words = words.split(" ")

words.forEach(i => {
 if( freq[i]) {
   freq[i] = freq[i] + 1
   } else {
     freq[i] = 1
     }
   })
 return freq
}

findOcc(sentence)
````

More: https://github.com/ChandaHubbard/wordOccurrences
