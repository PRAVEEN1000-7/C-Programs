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
//area and perimeter of square and rectangle
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
// to find out biggest number of three numbers
#include <stdio.h>
int main() {
    int x,y,z;
    printf("enter the x,y,z value :");
    scanf("%d %d %d",&x,&y,&z);
    if(x>y && x>z)
    {
        printf("%d is greater than %d and %d",x,y,z);
    }
    else if(y>x && y>z)
    {
        printf("%d is greater than %d and %d",y,x,z);
    }
    else
    {
        printf("%d is greater than %d and %d",z,x,y);
    }
    return 0;
}

----------------------------------------------------------------------------------------------------
sample input : 77 46 67
sample output :
enter the x,y,z value :77 46 67
77 is greater than 46 and 67

--------------------------------------------------------------------------------------------------
// average of odd number below a range 
#include <stdio.h>
int main() {
   int sum=0,x=0,num;
   
   printf("enter the range :");
   scanf("%d",&num);
   
   for(int i=0;i<=num;i++)
       {
           if(i%2==1)
          {
           sum=sum+i;
           x++;
         }
        }
   float aver= sum / x;
   
   printf("average of odd number for given number %d is %.2f",num,aver);
   return 0;
}

--------------------------------------------------------------------------------------------------
sample input : 9
sample output :
enter the range :9
average of odd number for given number 9 is 5.00

----------------------------------------------------------------------------------------------------
// perfect number 
#include <stdio.h>
int main() {
   int sum=0,num;
   
   printf("enter a number :");
   scanf("%d",&num);
   for(int i=1;i<num;i++)
   {
       if(num % i==0)
       {
           sum=sum+i;
       }
   }
   
   if(sum == num)
   {
       printf("given number %d is a perfect number",num);
   }
   else
   {
       printf("given number %d is not a perfect number",num);
   }
   return 0;
}

----------------------------------------------------------------------------------------
sample input : 6
sample output : 
enter a number :6
given number 6 is a perfect number

---------------------------------------------------------------------------------------
//  Net salary of an employee 
#include <stdio.h>

int main() {
    float net_sal,gro_sal,pro_tax,ppf,in_tax;
    printf(" enter the gross salary and professional tax :");
    scanf("%f %f",&gro_sal,&pro_tax);
    printf(" enter the public provident fund and income tax :");
    scanf("%f %f",&ppf,&in_tax);
    net_sal = gro_sal - pro_tax - ppf - in_tax;
    printf(" Net salary of an employee is : %.2f",net_sal);
    return 0;
}

----------------------------------------------------------------------------------------------
sample input :300000 12000 , 10000 21000
sample out  :
enter the gross salary and professional tax :300000 12000
enter the public provident fund and income tax :10000 21000
Net salary of an employee is : 257000.00

---------------------------------------------------------------------------------------
// result of a student 
#include <stdio.h>

int main() {
    int mark[5],per,a,b,c;
   
    printf("enter the 3 subject marks :");
    scanf("%d",&a,&b,&c);

    per=a+b+c/300*100;
    if(per>90)
    {
        printf(" grade A");
    }
    else if(per>75)
    {
        printf(" grade B");
    }
    else if(per>50)
    {
        printf(" grade C");
    }
    else if(per>35)
    {
        printf(" grade E");
    }
    else{
        printf(" grade F");
    }
    return 0;
}

----------------------------------------------------------------------------
sample input  : 97 90 99
sample output :
enter the 3 subject marks :97 90 99
grade A

---------------------------------------------------------------------------
// Vowels or not
#include <stdio.h>

int main() {
    char x;
    printf("enter the letter :");
    scanf("%c",&x);
    if(x=='a'||x=='i'||x=='o'||x=='e'||x=='u'||x=='A'||x=='I'||x=='O'||x=='E'||x=='U')
    {
        printf(" %c is a vowel.",x);
    }
    else
    {
         printf(" %c is not a vowel.",x);
    }
    return 0;
}

----------------------------------------------------------------------------
sample input : A
sample output : A is a vowel.

-----------------------------------------------------------------------------
// swapping of integers
#include <stdio.h>

int main() {
    int x,y,z;
    printf("enter the x value :");
    scanf("%d",&x);
    printf("enter the y value :");
    scanf("%d",&y);
    z=x;
    x=y;
    y=z;
    printf("x :%d\n",x);
    printf("y :%d",y);
    return 0;
}

----------------------------------------------------------------------------
sample input : 66 77
sample output : 
enter the x value :66
enter the y value :77
x :77
y :66

-----------------------------------------------------------------------------

// sum of digits of a number
#include <stdio.h>
int main () 
{
  int n,digit,sum=0;
  printf ("Enter number to findout sum of its digits: ");
  scanf("%d",&n);
  while(n!=0)
  {
       sum+=n%10;
     n=n/10;
  }
  printf ("the sum of digits of given number is %d",sum);
  return 0;
}

-------------------------------------------------------------------------------
sample input : 123456789
sample output :
Enter number to findout sum of its digits: 123456789
the sum of digits of given number is 45

----------------------------------------------------------------------------
//area of circle by user-defined function & call by value

#include<stdio.h>
float area(float x)// formal parameter
{
    float ar=3.14*x*x;
    return ar;
    
}
int main()
{
    float rad;
    printf("Enter the radius : ");
    scanf("%f",&rad);
    printf("Area of circle is %.2f\n",area(rad));//actual parameter
    return 0;
}

----------------------------------------------------------------------------
sample input and output :
Enter the radius : 7
Area of circle is 153.86

-----------------------------------------------------------------------------

//perimeter of circle by user-defined function & call by reference

#include<stdio.h>
float peri(float *x)// formal parameter
{
   *x=2*3.14**x;
     printf("Perimeter of circle is %.2f\n",*x);
    
}
int main()
{
    float rad;
    printf("Enter the radius : ");
    scanf("%f",&rad);
    peri(&rad);//actual parameter
    printf("after perimeter : %.2f ",rad);
    return 0;
}

-------------------------------------------------------------------------------

sample input and output :
Enter the radius : 7
Perimeter of circle is 43.96
after perimeter : 43.96 

---------------------------------------------------------------------------------
