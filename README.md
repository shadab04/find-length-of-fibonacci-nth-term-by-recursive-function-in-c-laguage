# find-length-of-fibonacci-nth-term-by-recursive-function-in-c-laguage
#include<stdio.h>
int fibonacci(int n);
int main()
{
   printf("%d\n",fibonacci(8));
    return 0;
}
int fibonacci(int n)
{
    if(n==0)
    {
        return 0;
    }
    if(n==1)
    {
        return 1;
    }
    int fibonacciNm1=fibonacci(n-1);
     int fibonacciNm2=fibonacci(n-2);
    int fibonacciN=fibonacciNm1+fibonacciNm2;
  //  printf("fibonacci of:%d\n%d",fibonacciN,n);
    return fibonacciN;
}
