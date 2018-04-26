/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>
void fun(int *p)
{
    int **ptr = p;
    int x;
    
    printf("%d, %d",p[0],p[1]);
    printf("\n%d, %d",&p[0],&p[1]);
    printf("\n%d, %d",&ptr[0],&ptr[1]);
    printf("\nSizeofint%d",sizeof(x));
    printf("\nSizeofp%d",sizeof(p));
    printf("\nSizeofptrptr%d",sizeof(ptr));
    //printf("%d, %d",p[0],p[1]);
}

void fun1(int **p)
{
    int *temp ;
    temp = (int*)p;
    
    printf("\n%d, %d",temp[0],temp[1]);
    //printf("%d, %d",p[0],p[1]);
    
}
int main()
{
    int m[3][3] = {{1,2,3},{4,5,6},{7,8,9}};
    fun1(&m[0][0]);
    //printf("\nHello World");

    return 0;
}
