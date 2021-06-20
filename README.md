# Number-of-set-bits-in-any-number-
#include <stdio.h>

int main()
{   int n,a;
    printf("Enter no that you want to count set bits:\n or hi User ek number do jiska set bits count karna hai:");
    scanf("%d",&n);
    int count=0;
    a=n;
   while(n>0)
   {
       if((n&1)==1)
       count++;
       n=n>>1;
   }
    printf("number of set bits in %d is %d",a,count);

    return 0;
}
