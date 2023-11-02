# c-practice-codes
// Online C compiler to run C program online
#include <stdio.h>

int main() {
   int n,temp = 0,max,min;
   scanf("%d", &n);
   
   int arr[n];
   for(int i=0; i<n; i++){
       scanf("%d", &arr[i]);
   }
for(int i=0; i<n; i++){
if (n%2==0){

 for(int i=0; i<n/2; i++){
     //arr[i]=arr[n-i-1];
     temp = arr[i];
     arr[i]= arr[n-i-i];
     arr[n-i-1]= temp;
     }
}

else
{
for(int i=0; i<(n-1)/2; i++){
     //arr[i]=arr[n-i-1];
     temp = arr[i];
     arr[i]= arr[n-i-i];
     arr[n-i-1]= temp;
     }
}
}
  for(int i=0; i<n; i++){
      printf("%d", arr[i]);
}
    return 0;
}
