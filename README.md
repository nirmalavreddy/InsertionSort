# InsertionSort
this a program for insertion sort
public class InsertionSort {

	public static void main(String[] args) {
		int[] a= {5, 1, 6, 2, 4, 3};
		
		int temp,j;
		/*1. select each element store it in temp
		 * 2. compare it with other elements and insert them in their correct position
		 */
		for(int i=1; i<a.length;i++)
		{
			temp=a[i];
			//we make some manipulations on j and since we don't want it to affect j we have considered i
			j=i;
			while(j>0 && a[j-1]>temp)
			{
				a[j]=a[j-1];
				j=j-1;
			}
			a[j]=temp;
		}
		for(int i=0; i<a.length;i++)
		{
			System.out.print(a[i]+" ");
		}
	}

}

