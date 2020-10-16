#include <stdio.h>

 float sumaver(x,y)
 {  
   float z;
    z=x+y;
    printf("The sum is %f\n",z);
    return z/2;
 }
 void even(x,y)
 {
     if(x%2==0)
     printf("%d is even\n",x);
     if(y%2==0)
     printf("%d is even\n",y);
 }
int main()
{   int a,b,c,l,sl;
    float avg;
      printf("Enter three numbers\n");
      scanf("%d%d%d",&a,&b,&c);
      fflush(stdin);
      if(a<b&&a<c)
      {
        l=b;
        sl=c;
      }
      else if(b<a&&b<c)
      {
          l=a;
          sl=c;
      }
      else
      {
          l=a;
          sl=b;
      }
    avg=sumaver(l,sl);
    even(l,sl);
    printf("The average is %f\n",avg);
    return 0;    
}
