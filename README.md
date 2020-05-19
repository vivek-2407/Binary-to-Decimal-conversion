# Python Program to get next prime number after a digit n
def prime(a):
    flag=0
    i=2
    while(i<a):
        if(a%i>0):
            i=i+1
            continue
        else:
            flag=1
            break
    if(flag==0):
        return(0)
    else:
        return(1)
def main():
    count=0
    n=int(input(print("Enter the number=")))
    while(count!=1):
        d=prime(n+1)
        if(d==0):
            count=1
        n=n+1
    print(n)
main()
