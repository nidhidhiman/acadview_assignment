### LEVEL-1

###### Q1. Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5,between 2000 and 3200 (both included).The numbers obtained should be printed in a comma-separated sequence on a single line.  

> Hints: Consider use range(#begin, #end) method

>###### Solution: l=[]
>###### for i in range(2000, 3201):
>######    if (i%7==0) and (i%5!=0):
>######        l.append(str(i))
>###### print ','.join(l)

###### Q2. Write a program which can compute the factorial of a given numbers. The results should be printed in a comma-separated sequence on a single line.

> Hints: In case of input data being supplied to the question, it should be assumed to be a console input.

###### Suppose the following input is supplied to the program: 8. Then, the output should be: 40320

>###### Solution:def fact(x):
>######    if x == 0:
>###### return 1
>######    return x * fact(x - 1)
>###### x=int(raw_input())
>###### print fact(x) 

###### Q3. With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary.
> Hints: In case of input data being supplied to the question, it should be assumed to be a console input.
> Consider use dict()
###### Suppose the following input is supplied to the program: 8.
###### Then, the output should be:
###### <pre> {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}.</pre>
 
>###### Solution:n=int(raw_input())
>###### d=dict()
>###### for i in range(1,n+1):
>######     d[i]=i*i
>###### print d

######  Q4.Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple which contains every number.

> Hints: In case of input data being supplied to the question, it should be assumed to be a console input. tuple() method can convert list to tuple
###### Suppose the following input is supplied to the program:34,67,55,33,12,98.
###### Then, the output should be:
###### <pre>['34', '67', '55', '33', '12', '98']</pre>
###### <pre>('34', '67', '55', '33', '12', '98')</pre>
 
>###### Solution: values=raw_input()
>###### l=values.split(",")
>###### t=tuple(l)
>###### print l
>###### print t

###### Q5.Write a program that accepts a comma separated sequence of words as input and prints the words in a comma-separated sequence after sorting them alphabetically.

> Hints:In case of input data being supplied to the question, it should be assumed to be a console input.

>###### Solution: items=[x for x in raw_input().split(',')]
>###### items.sort()
>###### print ','.join(items)

###### Q6. Write a program that accepts sequence of lines as input and prints the lines after making all characters in the sentence capitalized.
 
> Hints: In case of input data being supplied to the question, it should be assumed to be a console input.

###### Suppose the following input is supplied to the program:
###### <pre> Hello World
###### Practice makes perfect</pre>
###### Then, the output should be:
###### <pre> HELLO WORLD
###### PRACTICE MAKES PERFECT</pre>

>###### Solution: lines = []
>###### while True:
>######    s = raw_input()
>######    if s:
>######        lines.append(s.upper())
>######    else:
>######        break;
>###### for sentence in lines:
>######    print sentence

###### Q7.Write a program, which will find all such numbers between 1000 and 3000 (both included) such that each digit of the number is an even number. The numbers obtained should be printed in a comma-separated sequence on a single line.

>    Hints:<br><br>1. Use for loop with range().<br> 2. Use str() to convert int to str.<br>3. Use if Statement to obtain Output.

 ###### Q8.Write a program that accepts a sentence and calculate the number of letters and digits.
 >     Hints: Suppose the following input is supplied to the program:
 ###### <pre>hello world! 123</pre>
 ##### Then, the output should be:
 >###### <pre>LETTERS10
 >###### <pre>DIGITS 3

 ###### Q9.Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters.
 >##### Hints: Suppose the following input is supplied to the program:
 ###### <pre>HELLO WORLD!</pre>
 ##### Then, the output should be:
 >###### <pre>UPPER CASE 1
 >###### <pre>LOWER CASE 9

 ###### Q10.Use a list comprehension to square each odd number in a list. The list is input by a sequence of comma-separated numbers.
 >##### Hints: Suppose the following input is supplied to the program:
 ###### <pre>1,2,3,4,5,6,7,8,9</pre>
 ##### Then, the output should be:
 >###### <pre>1,3,5,7,9
