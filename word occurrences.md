Given a document, implement an algorithm to count the number of word occurrences.

Input: `"Hello there, how are you? Can you tell me how to get to the nearest Starbucks?"`

Output: `Hello = 1, there = 1, how = 2, are = 1, you = 2`

`const sent = "Hello there, how are you? Can you tell me how to get to the nearest Starbucks?"`

  `const replacePunc = (sentence, signs) => {
  let newSent = sentence;
  signs.forEach(sign => {
    newSent = newSent.replace(sign, '');
  })
  return newSent
}`
  
`function findOcc(sentence) {
  const sentPunc = replacePunc(sentence, ['?', ',', '?'])
  const sentArr = sentPunc.split(" ")
  let sentObj = { 
  }
  
  sentArr.forEach(item => {
    if (sentObj[item]) {
      sentObj[item] = sentObj[item] + 1
    } else {
      sentObj[item] = 1
    }  
  })
  return sentObj
}`

`findOcc(sent)`
