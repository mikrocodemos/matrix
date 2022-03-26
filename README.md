#include<stdio.h>
int main()
{
  int arr1[3][3],i,j,rows,col,sum=0;
  int *p=&arr1[i][j];
  printf("\n Please Enter Number of rows and columns  :  ");
 scanf("%d %d", &rows, &col);
  printf("Input elements in the matrix :\n");
  for(i=0;i<3;i++)
  {
      for(j=0;j<3;j++)
      {
	      printf("element - [%d],[%d] : ",i,j);
	      scanf("%d",&arr1[i][j]);
      }
  }  
  printf("\nThe matrix is : \n");
  for(i=0;i<3;i++)
  {
      printf("\n");
      for(j=0;j<3;j++)
           printf("%d\t",arr1[i][j]);
  }
 printf("\n\n");
 for(i=0;i<rows;i++)
    {
        for(j=0;j<col;j++)
        {
            if(i==j)
            {
                sum=sum+arr1[i][j];
            }
        }
    }
 
    printf("The sum of diagonal elements of a square matrix = %d\n",sum);
}
