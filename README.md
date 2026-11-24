#Q1. Reverse a String Problem Statement
n=input("Enter a string:")
rev=""
for ch in n:
  rev=ch+rev
print("The reversed string is",rev)

#Output:
Enter a string:Hello
The reversed string is olleH
Enter a string:python
The reversed string is nohtyp
Enter a string:12345
The reversed string is 54321


#Q2. Check Whether a String Is a Palindrome Problem Statement
n=input("Enter a string:")
temp=n
rev=""
for ch in n:
  rev=ch+rev
if rev==temp:
  print("It is a Palindrome")
else:
  print("It is not a Palindrome")

#Output:
Enter a string:madam
It is a Palindrome
Enter a string:level
It is a Palindrome
Enter a string:hello
It is not a Palindrome
Enter a string:121
It is a Palindrome


#Q3. Count Vowels and Consonants in a String Problem Statement
n = input("Enter a string: ")
vowels = 0
consonants = 0
for ch in n:
    if ('a' <= ch <= 'z') or ('A' <= ch <= 'Z'):
        if ch in "aeiouAEIOU":
            vowels += 1
        else:
            consonants += 1

print("The vowels are:", vowels)
print("The consonants are:", consonants)

#Output:
Enter a string: hello
The vowels are: 2
The consonants are: 3
Enter a string: Python
The vowels are: 1
The consonants are: 5
Enter a string: education
The vowels are: 5
The consonants are: 4
Enter a string: Hello123 World!
The vowels are: 3
The consonants are: 7


#Q4. Move Zeros to end
a=[0,10,2,3,0,0,0,3,0,0,2,4,5]
result=[]
for num in a:
  if num!=0:
    result.append(num)
for num in a:
  if num==0:
    result.append(num)
print(result)

#Output:[10, 2, 3, 3, 2, 4, 5, 0, 0, 0, 0, 0, 0]


#Q5. Find the difference between Largest and Smallest Element in array
a=[10,5,20,25,15]
largest=a[0]
smallest=a[0]
for num in a:
  if num>largest:
    largest=num
  elif num<smallest:
    smallest=num
print("The largest number is:",largest)
print("The smallest number is:",smallest)
print("The difference between largest and smallest number is:",largest-smallest)

#Output:
The largest number is: 25
The smallest number is: 5
The difference between largest and smallest number is: 20
