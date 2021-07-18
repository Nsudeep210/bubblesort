# bubblesort
/******************************************************************************

                              Online C++ Compiler.
               Code, Compile, Run and Debug C++ program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <iostream>

using namespace std;
void swap(int *xp,int *yp)
{int c =*xp;*xp=*yp;*yp=c;}

void bubs(int *arr, int n)
{int i,j;
for(i=0;i<n-1;i++)
{for(j=0;j<n-1-i;j++)
{if(*(arr+j)> *(arr+j+1))
swap(arr+j, arr+j+1);}}
}
int main()
{
    int arr[1]={2};int n=1;
for(int i=0;i<n;i++)
cout<<arr[i]<<",";
bubs(arr,n);
cout<<endl;
for(int i=0;i<n;i++)
std::cout<<arr[i]<<",";
    return 0;
}
