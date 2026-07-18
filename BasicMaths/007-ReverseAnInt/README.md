# 7. Reverse Integer

## Pattern
Digit Manipulation

## Difficulty
Medium

## Approach

- Extract the last digit using `% 10`
- Build the reversed number using
  rev = rev * 10 + digit
- Remove last digit using `/ 10`
- Use long to avoid overflow
- Return 0 if outside integer range

## Complexity

Time : O(log n)

Space : O(1)

## Revision Notes

Remember:
rev = rev * 10 + digit

Similar Problems
- 9. Palindrome Number
- 66. Plus One

## Mistake I Made:
Initially used int and checked overflow after reversing.

## What I Learned:
Using long avoids overflow. Another approach is to detect overflow before multiplication.

## Revision Trigger:
Whenever digits are extracted using %10 and removed using /10, think about rev = rev * 10 + digit.