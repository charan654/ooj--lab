#include <stdio.h>

int main()
{
     int a,b,d;
    int c;
    char ch;
    do
    {
    printf("Enter a and b\n");
    scanf("%d %d",&a,&b);
    printf("Enter the operation\n1-add\n2-subtract\n3-div\n4-multiply\n5-greater\n6-equality\n7-a is odd or even\n8-b is odd or even\n9-lesser\n10-not equal\n");
       scanf("%d",&c);
       
       switch(c)
       {
           case 1 : d=a+b;
                    printf("sum=%d\n",d);
                    break;
           case 2 : d=a-b;
                    printf("diff=%d\n",d);
                    break;
           case 3 : d=a/b;
                    printf("div=%d\n",d);
                    break;
           case 4 : d=a*b;
                    printf("multipication=%d\n",d);
                    break;
           case 5 : if(a>b)
                    printf("%d is greater than %d\n",a,b);
                    else
                    printf("%d is greater than %d\n",b,a);
                    break;
           case 6 : if(a==b)
                    printf("%d is equal to %d\n",a,b);
                    else 
                    printf("%d is not equal %d\n",a,b);
                    break;
           case 7 : if(a%2==0)
                    printf("%d is even\n",a);
                    else
                    printf("%d is odd\n",a);
                    break;
           case 8 : if(b%2==0)
                    printf("%d is even\n",b);
                    else
                    printf("%d is odd\n",b);
                    break;
          case 9  : if(a<b)
                    printf("%d is lesser than %d\n",a,b);
                    else
                    printf("%d is lesser than %d\n",b,a);
                    break;
          case 10 :if(a!=b)
                    printf("%d is not equal to %d\n",a,b);
                    else 
                    printf("%d is equal %d\n",a,b);
                    break;
       }
       printf("Do you want to continue? Enter Y or N\n");
       fflush(stdin);
       scanf("%c",&ch);
       }while(ch=='Y');

       return 0;
}
