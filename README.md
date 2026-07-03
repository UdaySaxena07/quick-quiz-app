# quick-quiz-app
A simple command-line quiz application built with Python.
q1='''What is the capital of India?
a)Mumbai
b)Delhi
c)kolkata'''
q2='''What is the english translation of kapde?
a)House
b)Rent
c)Clothes'''
count=0
score=0
l2=["b","c"]
l1=[q1,q2]
l3=["a","b","c"]
print("There will be a total of 2 question and each question is of 6 marks:")
for i in range(0,len(l1)):
    print(l1[i])
    str1=input("Type only a,b,c: ")
    if(str1!=l3[0] and str1!=l3[1] and str1!=l3[2]):
        print("Type only a,b or c")
        break
    if(str1==l2[i]):
        print("Correct answer")
        count=count+1
        score=score+6
    else:
        print("Wrong answer")
print(f"The score is {score}/{len(l1)*6}")
print(f"Your {count}/{len(l1)} are correct")
