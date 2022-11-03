# Lecture 0
- [Welcome](#welcome)
- [What is computer science?](#what-is-computer-science)
# Welcome
- This year, we’re back in Sanders Theatre, and David took CS50 himself as a sophomore years ago, but only because the professor at the time allowed him to take the course pass/fail.
- It turns out that computer science was less about programming than about problem solving. And though there may be frustration from feeling stuck or making mistakes, there will also be a great sense of gratification and pride from getting something to work or completing some task.
- In fact, David lost two points on his first assignment for not following all of the instructions correctly:
![](/pics/cs50-1.png)
    - And while this code (written in a programming language as opposed to a language like English) looks cryptic at first, it may only take weeks or months before we can understand main programming concepts and even teach ourselves new languages.
- Importantly,
    what ultimately matters in this course is not so much where you end up relative to your classmates but where you end up relative to yourself when you began
- In fact, two-thirds of CS50 students have never taken a computer science course before.
# What is computer science?
- Computer science is fundamentally problem solving, but we’ll need to be precise and methodical.
- We can think of **problem solving** as the process of taking some input (a problem we want to solve) and generate some output (the solution to our problem).
![](/pics/cs50-2.png)
- To begin doing that, we’ll need a way to represent inputs and outputs, so we can store and work with information in a standardized way.
## Representing Numbers
- To count the number of people in a room, we might start by using our fingers, one at a time. This system is called unary, where each digit represents a single value of one.
- To count to higher numbers, we might use ten digits, 0 through 9, with a system called decimal.
- Computers use a simpler system called binary, with just two digits, 0 and 1.
- For example, in binary this would be 0:

` 0 0 0 `
- And this would be 1:

` 0 0 1`

(We don’t need the leading zeroes, but we’ll include them to see the patterns more easily.)
- Since there is no digit for 2, we’ll need to change another digit to represent the next number:
` 0 1 0`
- Then we’ll “add 1” to represent 3:
`0 1 1`
- And continue the pattern for 4 …:
`1 0 0`
- … 5 …:
`1 0 1`
- … 6 …:
`1 1 0`
- … and 7:
`1 1 1 `
- Each binary digit is also called a bit.
- Since computers run on electricity, which can be turned on or off, we can simply represent a bit by turning some switch on or off to represent a 0 or 1.
- Inside modern computers, there are billions of tiny switches called transistors that can be turned on and off to represent different values.
- And the pattern to count in binary with multiple bits is the same as the pattern in decimal with multiple digits.
- For example, we know the following number in decimal represents one hundred and twenty-three.
`1 2 3`
    - The `3` is in the ones place, the `2` is in the tens place, and the `1` is in the hundreds place.
    - So `123` is `100×1 + 10×2 + 1×3 = 100 + 20 + 3 = 123`.
    - Each place for a digit represents a power of ten, since there are ten possible digits for each place. The rightmost place is for 100, the middle one 101, and the leftmost place 102:
    ![](/pics/cs50-3.png)
- In binary, with just two digits, we have powers of two for each place value:
![](/pics/cs50-4.png)
    - This is equivalent to:
    ![](/pics/cs50-5.png)
- With all the light bulbs or switches off, we would still have a value of 0:
![](/pics/cs50-6.png)
Now if we change the binary value to, say, 0 1 1, the decimal value would be 3, since we add the 2 and the 1:
