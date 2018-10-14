# w-10lab-a
#include<stdio.h>
#include<string.h>
int main()
{
    int n,i,a,b,flag,prod;

    int primeno(n)/*function to check prime no */
       {
           for(i=2;i<n;i++)
           if (n%i==0)
            {
               printf("%d IS NOT A PRIME NUMBER\n",n);
                  flag=1;
                     break;
            }


    if(flag=0)
        printf("%d is not a prime number",n);
    else

          {
            printf("%d is a prime number",n);
             for(i=1;i<=10;i++)
               {
                prod=n*i;
                 printf("%d\n",prod);
               }
         }


   }




     b=0;
    int armstrongno(n)
     {
    if(n>0)
      {while(n>0)
        a=n%10;
        b=b+a*a*a;
        n=n/10;
      if(b==n)
        printf("%d IS A ARMSTRONG NUMBER",n);
      else
        printf("%d IS NOT A ARMSTRONG NUMBER",n);
      }
    else(n<10&&n!=1);
        printf("%d IS NOT A ARMSTRONG NUMBER",n);
     }



  printf("ENTER A NUMBER:");
  scanf("%d",&n);

  primeno(n);
  armstrongno(n);
  return 0;
  }
