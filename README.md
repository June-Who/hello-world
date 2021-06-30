# hello-world
Just another repository

Hi human
=====Python practice https://www.practicepython.org/ ==============

7. List Comprehensions 
  Let’s say I give you a list saved in a variable: a = [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]. Write one line of Python that takes this list a and makes a new list that has only the even elements of this list in it. 
  Solution:
     a = [3, 4, 5, 6, 8, 0, 1, 88, 7, 3, 24]
    b = [x for x in a if x % 2 ==0]
    b.append( )
    print(b)
8. Rock Paper Scissors
  while 1:
    a = input('player a, please choose rock, paper or scissors ')
    b = input('player b, please choose rock, paper or scissors ')
    while a == 'rock':
        if b == 'rock':
            print('you are even')
        elif b == 'paper':
            print('b is the winner')
        elif b == 'scissors':
            print('a is the winner')
        else : print('please check your input')
        break

    while a == 'paper':
        if b == 'rock':
            print('b is the winner')
        elif b == 'paper':
            print('you are even')
        elif b == 'scissors':
            print('a is the winner')
        else:
            print('please check your input')
        break

    while a == 'scissors':
        if b == 'rock':
            print('b is the winner')
        elif b == 'paper':
            print('a is the winner')
        elif b == 'scissors':
            print('you are even')
        else:
            print('please check your input')
        break

    user_cmd = input('do you wish a new game? type "quit" to quit game')
    if user_cmd == "quit":
        break
    else: print('let us begin a new game')
  #note: could have used 'if a == b as a condition'
  
  
 9. Guessing Game One
  import random

n = 0
while 1:
    x = random.randint(1, 10)
    usr_cmd = input('please input a number or type "exit" to quit')
    if usr_cmd == "exit":
        break
    elif int(usr_cmd) > x:
        print('your guess is high')
        n = n+1
    elif int(usr_cmd) < x:
        print('your guess is low')
        n = n +1
    elif int(usr_cmd) == x:
        print('your guess is exactly right')
        n = n +1
    else:
        print('please type correctly, a number or "exit"')
        n = n+1
    print(x)

def test_prime():
    num = int(input('please give a number '))
    x = range(2, num)
    for e in x:
        i = 0
        if num % e == 0:
            i = i + 1
            if i != 0:
                print(e)
                print('your input is not a prime')
                break
    else :
        if e == num - 1:
            print('your input is a prime')


test_prime()

====== Practice 12 List Ends====
def list_ends(a):
    b = []
    b.extend([a[0],a[-1]])
    print(b)

test = [4,5,6,7,8,0,3]
list_ends(test)
==========Practice 13 Fibonacci============
def gen_fib(n):
    f = []
    i = 2
    if n == 1:
        f = [1]
    elif n == 2:
        f = [1,1]
    elif n >2:
        f.extend([1,1])
        while i < n:
            f.append(f[i-1] + f[i-2])
            i =i + 1
    print(f)

c = int(input('please type in a number '))
gen_fib(c)

==========END========================
