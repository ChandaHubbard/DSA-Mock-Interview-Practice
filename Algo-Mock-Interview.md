// 1. efficient solution
// 2. good use of data structure
// 3. complete solution

// k nearest stars to the earth (the earth is the origin)

// given a large list of stars (how to represent a star)
// given a number k

```
function hello() {
	return 'Hello world - JavaScript!';

	//sort each star based on distance, but checking each distance and placing it in the DS by deciding where is should go on based on the previous entries, time complexity n(log)n, very inefficient
	k = 1
	//go through the whole input list once, and check the distance of each, keep track of the minumum, return the minimum
	//how do you extend this solution to any k

	//let closestStars = starList[0]
	//now this should contain the first k items in the starList
	let closestStars = starList.slice(0, k-1)
	//start checking the array starList[k]
	//have an array
	for(let i = k; i < starList.length - k; i++) {
		for(let j = 0; j < closestStars.length; j++)
			if(starList[i] < closestStars[j]) {
			closestStar.push(starList[i])
		}
	}
	return closestStars
  }
  ```
	// 1.start from the solution for k = 1 case
	// do the same process k times
	//remember what star you returned so far, then exclude that from the next iteration
