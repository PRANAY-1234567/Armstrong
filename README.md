🔢 Armstrong Number Checker in Python
📌 Description

This program checks whether a given number is an Armstrong Number or not.

An Armstrong Number is a number where the sum of its digits raised to the power of the total number of digits is equal to the number itself.

🧩 Problem Statement

Given a number:

153


Check if it is an Armstrong Number.

✅ What is an Armstrong Number?

A number is called an Armstrong Number if:

𝑑
𝑖
𝑔
𝑖
𝑡
1
𝑛
+
𝑑
𝑖
𝑔
𝑖
𝑡
2
𝑛
+
𝑑
𝑖
𝑔
𝑖
𝑡
3
𝑛
+
.
.
.
=
𝑛
𝑢
𝑚
𝑏
𝑒
𝑟
digit1
n
+digit2
n
+digit3
n
+...=number

Where n is the total number of digits.

Example:

For 153:

1
3
+
5
3
+
3
3
=
153
1
3
+5
3
+3
3
=153

So, 153 is an Armstrong Number.

✅ Code
num = 153
temp = num
sum = 0

digits = len(str(num))

while temp > 0:
    digit = temp % 10
    sum += digit ** digits
    temp = temp // 10

if sum == num:
    print("Armstrong Number")
else:
    print("Not Armstrong Number")

🧠 Explanation

digits = len(str(num)) finds the number of digits

temp stores a copy of the original number

The while loop extracts each digit using % 10

Each digit is raised to the power of total digits

The results are added together

If the final sum equals the original number → Armstrong Number

🖨 Example Output
Armstrong Number

🛠 Concepts Used

Loops (while)

Modulus operator (%)

Integer division (//)

Power operator (**)

Number logic

🎯 Use Cases

Interview preparation

Number-based logic practice

Beginner Python exercises

Competitive programming basics

🚀 Possible Improvements

Take user input

Check Armstrong numbers in a range

Convert into a reusable function

👨‍💻 Author

Pranay Jadhao
