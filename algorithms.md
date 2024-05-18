
Sure, here's the formatted text in Markdown:

Sorting Algorithms:
No sorting algorithms provided.

Searching Algorithms:
Binary Search:
javascript

//function binarySearch(searchList, value) {
    let arrayPath = [];
    let left = 0;
    let right = searchList.length - 1;
    let middle = Math.floor(right / 2);

    // Search for target value
    while (searchList[middle] !== value) {
        arrayPath.push(searchList[middle]);

        // Search for value not found
        if (right < left) {
            return 'Value Not Found';
        }

        // Value is in left or right portion of array
        // Update L - M - R
        if (searchList[middle] > value) {
            right = middle - 1;
            middle = left + Math.floor((right - left) / 2);
        } else {
            // If the middle is smaller than the target, the middle now becomes the left.
            left = middle + 1;
            middle = left + Math.floor((right - left) / 2);
        }
    }

    // Add target value to output array
    arrayPath.push(searchList[middle]);

    return arrayPath;
}
