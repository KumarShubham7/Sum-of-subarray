# Sum-of-subarray

import java.util.*;
class HelloWorld
{
	public static void main(String[] args) {
	    
	    Scanner op = new Scanner(System.in);
	    System.out.println("Enter the sum u want to find:- ");
	    int s = op.nextInt();
		
		int A[] = {1,2,3,7,5};
		int i,j,k;
		int n=5;
		int sum=0;
		int flag=0;
		
		for(i=0;i<n;i++)
		{
		    for(j=i+1;j<n;j++)
		    {
		        for(k=j+1;k<n;k++)
		        {
		             sum = A[i]+A[j]+A[k];
		            j++;
		            i++;
		            
		            if(s==sum)
		            {
		                System.out.println("");
		                System.out.print(i+" ");
		                System.out.print(k+1);
		                flag++;
		            }
		            
		        }
		        break;
		    }
		    break;
		}
		if(flag==0)
		System.out.println("Sum not found");
	
	}
}
