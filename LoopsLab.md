# Loops Lab, Fri.6.28.19 - Blanca Cruz 6.1

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**

var allNumbers = 1

while allNumbers < 150 {
allNumbers += 1
print (allNumbers)
}

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

let rangeNumbers = 142...159

var AllNumbers = 0

for i in rangeNumbers {
print (i)
}

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

let rangeNumbers = 15...80

for i in rangeNumbers {
if i % 2 == 0 {
print(i)}
}

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

let rangeNumbers = 19...51

for i in rangeNumbers {
if i % 2 != 0 {
print(i)}
}

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

var rangeOfNumbers = 0...100
var index = 0

while rangeOfNumbers.contains(index) {
index += 5
print(index)
}

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

var rangeOfNumbers = 1...40
var index = 0

for index in rangeOfNumbers {
if index % 10 == 7 {
print(index)}
}

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

var rangeOfNumbers = 20...150
var index = 0

for index in rangeOfNumbers {
if index % 3 == 0 {
print(index)}
}

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

var rangeOfNumbers = 20...150
var i = 0

for i in rangeOfNumbers {
if i % 2 == 0 && i % 3 == 0 {
print(i)}
}

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`


var rangeOfNumbers = 20...150
var index = 0

for index in rangeOfNumbers {
if index % 10 == 4 {
print(index)}
}

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

var rangeOfNumbers = 20...150
for i in rangeOfNumbers {

if i == 31 || i == 35 || 40 <= i && i <= 60 {
print(i)}
}

***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

Answer: an infinite loop

// Your explanation here
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i < 9) {
    i += 1
}
```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 0

while (i < 1000) {
i += 1
print(i)
}

```

***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 0

while (i < 1000) {
i += 1
if i % 2 == 0 {
print(i)}
}
```

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift

Answer: The difference between Loop 1 & 2 is the "repeat" function. Both loops have the same outputs using string interpolation as well. 

var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```

***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.

Answer: Break function has limitations and stop once it finds its corresponding true statement. The Continue function is the opposite; it runs into the condition is met. 

for i in 2...20 {
if (i >= 5 && i <= 10){
continue
}
print(i)
}


***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}


for i in 2...10 {
if (i >= 6 && i <= 8){
break
}
print(i)
}

```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[x]8
[x]9
[x]10

***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}

It's checking the if condition of "y" when it is true it will continue to the outerloop. It will never print the interloop. 
```

***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

outerloop: for x in 1...10 {
innerloop: for y in 1...10 {
print("x = \(x), y = \(y)")
}
}

***
## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

var a = 10

outerloop: for x in 0...a {
innerloop: for y in 0...a {
if x - y <= 5 {
print("x = \(x), y = \(y)")
}
}
}

***
## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift

var N = 5
var i = 1

while i<=N {
print(i * i)
i += 1
}

1
4
9
16
25
```

***
## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
var n = 2
var m = ""
var i = 0

for _ in i..<n {
for _ in i..<n {
m+="*"
i+=1
}
print(m)
}

**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
