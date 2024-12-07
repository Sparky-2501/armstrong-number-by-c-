# armstrong-number-by-c-
#include <stdio.h>
#include<math.h>

void main()
{
    int n;
    printf("enter your number:");
    scanf("%d", &n);
    
    int N = n , num1 = n , x = 0;
                
        // 1]count of digits  
                int count=1;
                for(int i=1 ; i<n; i++)
                 {
                   count++;
                   n/=10;
                 }
                
        // 2] armstrong number 
        
                int singledigit, power;
                for( int i=1 ; i<=count ; i++)
                 {
                   singledigit=N%10;
                   power=pow(singledigit , count);
                   x=x+power;
                   N=N/10;
                 }
                 
                 
                  if(num1==x)
                    printf("it is armstrong number");
                  else
                    printf("it is not armstrong number");
    
}
