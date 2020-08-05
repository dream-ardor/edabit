## Shortest Unsorted Continuous Subarray

Given an integer array, you need to find the shortest continuous subarray that if you only sort this subarray in ascending order, then the whole array will be sorted in ascending order, too.

Create a function that returns the length of that subarray.
```
Examples
findUnsortedSubarray([1, 3, 2, 5, 8, 7, 13]) ➞ 5
// You need to sort [3, 2, 5, 8, 7] in ascending order to make
// the whole array sorted in ascending order.

findUnsortedSubarray([10, 7, 5, 3]) ➞ 4

findUnsortedSubarray([2, 4, 4, 4, 4, 3]) ➞ 5
```
### :computer: My Code
```js
let findUnsortedSubarray = n => {
    let c = [...n];
    c.sort((a,b)=>a-b);
    let i = 0; j = n.length-1;
    if(n.length===1) return 0;
    while(i<j && (c[i]===n[i]||c[j]===n[j])){
        if(c[i]===n[i]){
            i++;
        }
        if(c[j]===n[j]){
            j--;
        }
        if(i>=j) return 0;
    };
    return j-i+1;
};

//alternate
const findUnsortedSubarray = nums => {
 if (nums[0]== Math.min(...nums)) return findUnsortedSubarray(nums.slice(1))
 if (nums[nums.length-1]== Math.max(...nums)) return findUnsortedSubarray(nums.slice(0,-1))
 return nums.length;
};
```
