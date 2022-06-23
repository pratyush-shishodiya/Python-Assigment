# Python-Assigment
#!/usr/bin/env python
# coding: utf-8

# 1


str1="Pratyush"
str2=str1.replace("P","p")
str2


# 2



str1="My naaaame is pratyush."
str2="a";
count=0
for i in range(len(str1)):
    if(str2==str1[i]):
        count=count+1
    
print(count)
    


# 3


def count_occ(ch,str1):
    count=0
    for i in range(len(str1)):
        if(ch==str1[i]):
            count=count+1
    print(count)
str1="My naaaame is pratyush."
ch="a"
count_occ(ch,str1)








# 4



def anagram(str1,str2):
    count=0
    for i in range(len(str1)):
        for j in range(len(str2)):
            if(str1[i]==str2[j]):
                count=count+1
    if(count==len(str1)):
        return "Yes"
    else:
        return "No"
    
str1="abcdb"
str2="dbcab"
anagram(str1,str2)


# 5


def anagram(st1,str2):
    sortstr1=sorted(str1)
    sortstr2=sorted(str2)
    
    if(len(str1)==len(str2)):
        if(sortstr1==sortstr2):
            return "Yes"
        else:
            return "No"
    else:
        return "No"
str1="abcdb"
str2="dbcab"
anagram(str1,str2)     


# 6



def palidrome(str):
    if(str==str[: :-1]):
        return "Yes"
    else:
        return "No"
    
str="civi"
palidrome(str)


# 7


def vowel(str):
    if(str=="A" or str=="E" or str=="I" or str=="O" or str=="U" or str=="a" or str=="e" or str=="i" or str=="o" or str=="u"):
        return "Yes"
    else:
        return "No"
str="A"
vowel(str)


# 8


ch="y"
print(ord(ch))





def isdigit(ch):
    if(ord(ch)>=48 and ord(ch)<=57):
        return "Yes"
    else:
        return "No"
    
ch="q"
isdigit(ch)


# 9


def replacespace(ch,str):
    str2=str.replace(' ',ch)
    return str2
str='Pratyush singh shishodiya '
ch="|"
replacespace(ch,str)


# 10


str="Pratyush singh shishodiya"
ch='-'
res=''

for i in str:
    if i==' ':
        i=ch
    res+=i
print(res)


# 11


str="pratyush"
str1=str.upper()
print(str1)


# 12


str="PRATYUSH"
str1=str.lower()
print(str1)


# 13


lis=list(range(1,101))
print(lis)


# 14


def miss(arr,n):
    total=((n+1)*(n+2))/2
    sum_of_arr=sum(arr)
    missing_number=total-sum_of_arr
    return missing_number

arr=[1,2,3,4,6,7]
n=len(arr)
miss(arr,n)
    


# 15


def dup_num(arr):
    arr.sort()
    for i in range(0,len(arr)):
        for j in range(i+1,len(arr)):
            if arr[i]==arr[j]:
                print(arr[j])
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3];
dup_num(arr)


# 16


def sum_pair(arr,n):
    count=0
    for i in range(0,len(arr)):
        for j in range(i+1,len(arr)):
            if arr[i]+arr[j]==n:
                count=count+1
                print(arr[i],arr[j])
        return count
arr=[1, 5, 7, -1,5]
n=6
sum_pair(arr,n)


# 17


def check_size(arr1,arr2):
    if(len(arr1)==len(arr2)):
        return "Equal"
    else:
        return "Not equal"
arr1=[1,2,3,4]
arr2=[5,6,7,8]
check_size(arr1,arr2)


# 18


def max_ele(arr):
    arr.sort()
    n=len(arr)
    print(arr[n-1])
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3]
max_ele(arr)


# 19


def max_ele(arr,n):
    max=arr[0]
    for i in range(1,n):
        if arr[i]>max:
            max=arr[i]
        return max
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3]
n=len(arr)
max_ele(arr,n)


# 20


def max_ele(arr):
    arr.sort()
    n=len(arr)
    print(arr[n-2])
arr=[1, 2, 3, 4, 2, 7, 8, 3]
max_ele(arr)


# 21


def max_ele(arr):
    arr.sort()
    n=len(arr)
    print(arr[n-1],arr[n-2])
arr=[1, 2, 3, 4, 2, 7, 8, 3]
max_ele(arr)


# 22


def dup_num(arr):
    arr=set(arr);
    print(arr)
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3];
dup_num(arr)


# 23


def print_rev(arr,n):
    for i in range(n-1,0,-1):
        print(arr[i])
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3]
n=len(arr)
print_rev(arr,n)


# 24


def length(arr):
    count=0
    for i in arr:
        count=count+1;
    return count
arr=[1, 2, 3, 4, 2, 7, 8, 8, 3]
length(arr)


# 24


arr=[1, 2, 3, 4, 2, 7, 8, 8, 3]
arr.append(10)
arr







