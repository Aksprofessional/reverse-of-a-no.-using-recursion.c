# reverse-of-a-no.-using-recursion.c
// C program  to print reverse of a given no. using recursion with functions.
// C program  to print reverse of a given no. using recursion with functions

#include <stdio.h>
int rev(int);
int main() {
    int n,r;
    printf("enter number=");
    scanf("%d",&n);
    rev(n);
    return 0;
}
int rev(int n){
    int r;
    if(n==0)
    return 0;
    r=n%10;
    printf("%d",r);
    rev(n/10);
}
