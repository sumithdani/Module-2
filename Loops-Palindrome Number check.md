## Loops in Python: Palindrome Number Checker

##  Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
reverse = 0
while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num = num // 10
if temp == reverse:
    print("Palindrome Number")
else:
    print("Not a Palindrome Number")
```
## Output
<img width="248" height="147" alt="image" src="https://github.com/user-attachments/assets/78537d60-9ca4-4e8b-b9bc-68bc2ed8323f" />

## Result
Thus, the Python program to check whether a given number is a palindrome using loops was executed successfully.
