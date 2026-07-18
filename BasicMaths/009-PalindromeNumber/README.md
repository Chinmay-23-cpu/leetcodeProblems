# 7. Reverse Integer

## Pattern
Digit Manipulation

## Difficulty
Easy

## Approach
- Store the original number in a separate variable.
- Extract the last digit using `% 10`.
- Build the reversed number using:
  reverse = reverse * 10 + digit
- Remove the last digit using `/ 10`.
- Compare the reversed number with the original number.
- Return `false` for negative numbers.

## Complexity

Time : O(log n)

Space : O(1)

## Revision Notes

Remember:
- Store the original number before modifying it.
- Reverse the number using:
  reverse = reverse * 10 + digit
- Compare the reversed number with the original.

Similar Problems
- 7. Reverse Integer
- 66. Plus One
- 415. Add Strings

## Mistake I Made:
- Initially compared the reversed number with `x`.
- Forgot that `x` becomes `0` after the loop.
- Fixed it by storing the original value before modifying `x`.

## What I Learned:
- Reused the digit extraction pattern from **Reverse Integer**.
- Learned that modifying the input variable means I need to preserve its original value for comparison.
- Negative numbers are never palindrome numbers.
