# PlusOne

## Example 1:
```
Input: digits = [1,2,3]
Output: [1,2,4]
Explanation: The array represents the integer 123.
```
## Example 2:
```
Input: digits = [4,3,2,1]
Output: [4,3,2,2]
Explanation: The array represents the integer 4321.
```
## Example 3:
```
Input: digits = [0]
Output: [1]
```
## Solution

#### JavaScript
```
var plusOne = function(digits) {
    for (let i = digits.length - 1; i >= 0; --i) {
        console.log(i);
        if (digits[i] < 9) {
            digits[i]++;

            return digits;
        } else {
            digits[i] = 0;
        }
    }

    digits.unshift(1);
    return digits;
};
```