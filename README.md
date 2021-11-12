#include<stdio.h>

int foo(int max, int a, int b)

{

   

  while(1)

  {

    if(max%a==0 && max%b==0)

    {

      return max;

      break;

    }

    else

    {

      foo(++max,a,b);

    }

  }

}

 

 int main()

 {

   int a,b,lcm,max;

   printf("enter the 2 numbers \n");

   scanf("%d %d",&a,&b);

   max=(a>b?a:b);

   printf("the lcm is %d",foo(max,a,b));

   return 0;

 }
