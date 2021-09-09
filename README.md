#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() 
{

    int n;
    scanf("%d", &n);
    int length=n*2-1;
    int arr[length][length];
  	for (int i=0; i<n; i++) {
      for (int j=i; j<length-i; j++) {
      arr[i][j]=n-i;
      arr[length-i-1][j]=n-i;
      arr[j][i]=n-i;
      arr[j][length-i-1]=n-i;
      }
    
      }
      for (int i=0; i<length; i++) {
      for (int j=0; j<length; j++) {
      
      printf("%d ", arr[i][j]);
      }
      printf("\n");
      }
    return 0;
}
