# c-7
Array program to delete a value
#include<stdio.h>
int main()
{
    int n,i,pos;
    printf("enter no.");
    scanf("%d",&n);
    int arr[n];
    printf("enter elements");
    for(i=0;i<n;i++)
    {
    scanf("%d",&arr[i]);
    }
    printf("enter the element position to delete:");
    scanf("%d",&pos);
    if(pos<1||pos>n){
        printf("invalid position");
        return 1;
    }
    for(i=pos-1;i<n-1;i++)
    {
        arr[i]=arr[i+1];
    }
    n--;
    printf("after deletion:\n");
    for(i=0;i<n;i++)
    {
        printf("%d \t",arr[i]);
    }
    printf("\n");
    return 0;
   }
