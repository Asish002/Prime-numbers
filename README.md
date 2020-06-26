# Prime-numbers
#include <stdio.h>

int main() {
   int x,i,c=0,k=0,j[2000],l=0;
   for(x=1;x<=10000;x++)
   {
    for(i=1;i<=x;i++)
    {
      if((x%i)==0)
      {
         c++;
      }
    }
    if(c==2)
    {
      j[k]=x;
      printf("%d\n",j[k]);
      l++;
      k++;
    }
    c=0;
   }
   printf("length=%d",l);
   return 0;
}
