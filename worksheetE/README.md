a)
```
num1 = 5
num2 = 7

result = 0 + 0
i = num1 + 0

while i != 0:
    result = result + num2
    i = i - 1

print(result)
```

b) The code has the effect of multiplying the values in $0 and $1, because the code runs through the while loop for 5 times (the value of
num1, and therefore, in my code $0), each time 7 is added to the result. So, effectivly, 7 is added 5 times, leaving us with 5 x 7 = 35.

c) 
```
inputNumber = 10
finalResult = 1

while inputNumber != 0:

    tempResult = 0
    i = inputNumber
    while i != 0:
        tempResult = tempResult + finalResult
        i = i - 1
    finalResult = tempResult
    inputNumber = inputNumber - 1

print(finalResult)
```

d) The inner loop completes one less iteration for each iteration of the outer loop. If the inputNumber is 4, the outer loop iterates 4
times, whilst the inner loop will iterate 4 times, then 3 times, then 2 times, then once. The inner loop multiples the current total, as stored in tempResult, with the value of i, for each outer loop iteration. At each stage, the inner loop multiples the current interger in tempResult with the product of all previous intergers leading up to it and then on the completion of all loops, the total for these multiplcations is stored in finalResult and printed.

e)
```
           addi $s0, $zero, 10
            addi $s1, $zero, 1
inner: mult $s1, $s0
            mflo $s1
            addi $s0, $s0, -1
            bne $s0, $zero, inner
```
