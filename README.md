# insertion_sort

package elclipse;
import java.util.*;
public class Insertion_sort {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {5,4,9,8,3,2,1};   ///initializing array
		int temp,j;
		for(int i=1;i<a.length;i++) {
			temp=a[i];
			j=i;
			while(j>0 && a[j-1]>temp) {             //camparing element with previous element
				a[j]=a[j-1];                       
				j=j-1;
			}
			a[j]=temp;
		}

		System.out.print(Arrays.toString(a));                ///converting arrays to string

	}
}

///time complexity of insertion sort is o(n^2).
