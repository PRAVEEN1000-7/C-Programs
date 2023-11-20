// multiplication table of given number and range 

#include <stdio.h>
int main() {
    int x,y;
    printf("enter the range :");
    scanf("%d",&x);
    printf("enter the number :");
    scanf("%d",&y);
    for(int i=0;i<=x;i++)
    {
        printf("%d x %d = %d\n",y,i,y*i);
    }
    return 0;
}

------------------------------------------------------------------------------------------------

sample input : 20 7
sample output :
enter the range :20
enter the number :7
7 x 0 = 0
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
7 x 9 = 63
7 x 10 = 70
7 x 11 = 77
7 x 12 = 84
7 x 13 = 91
7 x 14 = 98
7 x 15 = 105
7 x 16 = 112
7 x 17 = 119
7 x 18 = 126
7 x 19 = 133
7 x 20 = 140

-------------------------------------------------------------------------------------

// even number upto a range 
#include<stdio.h>
int main()
{
    int x,even;
    scanf("%d",&x);
    for(int i=1;i<=x;i++)
    {
        if(i%2==0)
        {
            even+=i;
        }
    }
    printf("%d",even);
    return 0;
}

------------------------------------------------------------------------------------------
sample input : 5
sample output: 6

-------------------------------------------------------------------------------------------

#include <stdio.h>
int main() {
    int sq,sq2,rec,x,l,b,rec2;
    printf("enter the x value for square:");
    scanf("%d",&x);
    printf("enter the length for rectangle :");
    scanf("%d",&l);
    printf("enter the breadth for rectangle:");
    scanf("%d",&b);
    sq=x*x;
    sq2=4*x;
    rec=l*b;
    rec2=2*(l+b);
    printf("area of square is %d \nperimeter of square is %d\n",sq,sq2);
    printf("\narea of rectangle is %d \nperimeter of rectangle is %d",rec,rec2);
    return 0;
}

----------------------------------------------------------------------------------------------
sample input : 5,10,4
sample output : 
enter the x value for square:5
enter the length for rectangle :10
enter the breadth for rectangle:4
area of square is 25 
perimeter of square is 20

area of rectangle is 40 
perimeter of rectangle is 28

-----------------------------------------------------------------------------------------------

