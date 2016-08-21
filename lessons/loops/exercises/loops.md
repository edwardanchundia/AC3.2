## A) For each prompt below, write a for loop that prints out the specified information.

1) All the numbers from 1 to 150 inclusive

for i in 1...150 {
    print (i)
}

2) All the numbers from 142 to 159 exclusive

for i in 142..<150 { 
    print (i)
}

3) Only the even numbers from 15 to 80 inclusive

for i in 15...80 {
    if i%2==0{
        print (i)
    }
}

4) Only the odd numbers from 19 to 51 inclusive

for i in 19...51 {
    if i%2==1{
        print (i)
    }
}

5) All the numbers that end in a 5 from 1 to 100 exclusive

for i in 1..<100 {
    if i % 5 == 0 && i % 10 != 0 {
        print (i)
    }
}

6) All the numbers that end in a 7 from 1 to 40 inclusive

for i in 1...90 {
    if i % 5 == 2 && i % 2 != 0{
       print(i)
   }
}


## B) Given a range of numbers from 20 to 150 print out all the numbers that follows these conditions

1) Numbers that are divisible by 3

for i in 20...150 {
    if i % 3 == 0 {
       print(i)
   }
}

2) Numbers that are divisible by 2 and 3

for i in 20...150 {
    if i % 2 == 0 && i % 2 == 0 {
       print(i)
   }
}

3) Unit digit ends with 4

for i in 20...150 {
    if (i - 4) % 10 == 0 {
       print(i)
   }
}

4) Print out numbers contain 31, 35, 40 to 60.


for i in 20...150 {
    switch x {
        case 31, 35, 40...60, 131, 135, 140..150:
        print (i)
    befault:
        break
    }
}



## C) While loop (NO Xcode)
```
var i = 5
while (i > 3) {
  i += 1
}
```
1) How many times does this while loop execute?

infinite

2) How do you stop the loop when i reaches 9?

change conidtion to i <= 9

3) How would you fix the while loop so that it only execute 1,000 times.

change condition to i <= 1005

4) Once the loop can run 1,000 times, print out ONLY the even number.

add if i % 2 = 0 print i

```
var i = 1
while i <= 10 {
    print("i = \(i)")
    i+=1
}
```
```
var i = 1
do {
   print("i = \(i)")
   i+=1
} while i <= 10
```

5) What's the difference between these two while loop?


The frist one does it ten times and the second 

6) If there's a difference, how would you fix it so that both outputs are the same.


## D) Short Answer Questions (NO Xcode)

1) What's the difference between break vs continue?

break will completely stop the code as for continue it will execute again

2) Without using Xcode explain the result of the following for-in loops.
* a)
```
for i in 1...10 {
    if (i >=4 && i <= 7){
        continue
    }
    print(i)
}
```

will print 4, 5, 6, 7 


* b)
```
for i in 1...10 {
    if (i >=4 && i <= 7){
        break
    }
    print(i)
}
```

will print 1,2,3


* Bonus)
```
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}



```
##E) Nested loops
1) Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) where x and y are both integers.

for x in 1...5 {
for y in 1...5 {
print("\(i),\(j)", separator: "", terminator: " ")
}
print("")
}

2) Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) where x and y are both even numbers.

for x in 0...10 {
for y in 0...10 {
if x % 2 == 0 && y % 2 == 0 {
print("\(x),\(y)", separator: "", terminator: "")
}
print("")
}
}

3) Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) where the difference of x and y is at least 5, and x and y are both integers.

for x in 0...10 {
for y in 0...10 {
if x % 2 == 0 && y % 2 == 0 {
print("\(x),\(y)", separator: "", terminator: "")
}
print("")
}
}

4) Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) where the product of x and y is less than 6, and x and y are both integers.

for x in 0...10 {
for y in 0...10 {
if x % 2 == 0 && y % 2 == 0 {
print("\(x),\(y)", separator: "", terminator: "")
}
print("")
}
}

5) Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) where the x is not equal to y and x and y are both integers.

for x in 0...10 {
for y in 0...10 {
if x != y {
print("\(x),\(y)", separator: "", terminator: "")
}
print("")
}
}

