# Python-Lingusitics
def isometric(st1,st2):
    if len(st1)!=len(st2):
        return False
    else:
        dic1={}
        dic2={}
        for i in range(len(st1)):
            char1=st1[i]
            char2=st2[i]
            if char1 not in dic1:
                dic1[char1]=char2
            if char2 not in dic2:
                dic2[char2]=char1
            if dic1[char1]!=char2 or dic2[char2]!=char1:
                return False
    return True
st1=input("Enter your 1st String:")
st2=input("Enter Your Second String:")
print(isometric(st1,st2))
        
    
