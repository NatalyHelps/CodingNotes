sorting algorithms:

searching algorithms:
Binary Search:
`function binarySearch(searchList, value) {

let arrayPath = [];
let left = 0;
let right = searchList.length - 1;
let middle = Math.floor(right/2);

//search for target value

while(searchList[middle] !== value) {
    arrayPath.push(searchList[middle]);
    
//SEARCH FOR VALUE NOT FOUND - if right is smaller than left it means the search space isn't valid - no elements left to check - termination condition, means the target value is not present in the array
      if (right < left) {
       return 'Value Not Found';
    }

// value is in left or right portion of array
// update L - M - R
if (searchList[middle] > value) {
  right = middle - 1;
  middle = left + Math.floor((right - left) / 2);

//right-left would give you the length of the search range. And then dividing it by 2 would be cutting it in half. 
} else {
//if the middle is smaller than the target, the middle now becomes the left. 
  left = middle + 1;
  middle = left + Math.floor((right - left) / 2);

  }
}
  // add target value to output array  
  arrayPath.push(searchList[middle]);

  return arrayPath;
}`
