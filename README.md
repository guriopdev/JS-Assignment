# JS-Assignment
1. Count Numbers Divisible by K

Given integers L, R, and K, count how many numbers in the range [L, R] are divisible by K.

Approach:
Iterate from L to R, check divisibility using modulo, and maintain a counter.

Time Complexity: O(R - L)
Space Complexity: O(1)

2. Digit Constraints with Prime Sum

Count numbers in a range that:

Are divisible by K
Do not contain digit 0
Have a sum of digits that is prime

Approach:
For each number:

Extract digits using modulo and division
Skip if any digit is 0
Compute digit sum
Check if sum is prime

Time Complexity: O(R - L)
Space Complexity: O(1)

3. Roll-Seed Lock

Apply transformations to a number N for 3 steps:

If even → N = N/2 + seed
If odd → N = N*3 - seed

After 3 steps:

Check if result is a 3-digit number
Check if middle digit equals seed

Approach:
Use a loop running exactly 3 times and apply conditions accordingly. Extract middle digit using division.

Time Complexity: O(1)
Space Complexity: O(1)

4. Mirror Corridor

Find the smallest non-negative integer X such that:

N + X is a palindrome
N + X is divisible by K

If no such X exists within 0 ≤ X ≤ 100000, return -1.

Approach:

Iterate X from 0 to 100000
Check divisibility
Check palindrome using numeric reversal

Time Complexity: O(100000 × digits)
Space Complexity: O(1)

5. Fare Calculator

Compute ride fare using multiple rules:

Base fare calculation
Late penalty
Distance-based percentage addition
Seed-based adjustment
Round up to nearest multiple of 5

Approach:
Apply conditions in strict order and use arithmetic tricks to round up without built-in functions if required.

Time Complexity: O(1)
Space Complexity: O(1)

6. Skipping Numbers

Find the smallest integer m such that the sum of numbers from 1 to m (excluding multiples of seed + 2) is at least N.

Approach:

Iterate numbers starting from 1
Skip multiples of (seed + 2)
Accumulate sum until it reaches or exceeds N

Time Complexity: O(m)
Space Complexity: O(1)

7. Contest Score Judge

Compute a score using:

score = 3a + b - 2c

Apply rules:

If negative, set to 0
If total submissions exceed 50, subtract 10
Determine PASS or FAIL based on final score

Approach:
Direct computation with conditional checks.

Time Complexity: O(1)
Space Complexity: O(1)
