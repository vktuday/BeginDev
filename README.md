package coreJavaPractice;
import java.util.ArrayList;

import org.junit.Test;


public class Collections
// an array is collection of similar data types
{
	@Test
public void staticIntArray()
{
  int[] numbers = {1,2,3,4,5,6,7};
  int  len = numbers.length;
  System.out.println("Lenght of array:" +len);
  int firstnum =numbers[0];
  for(int i=0;i<len;i++)
  {
	        int StdNum = numbers[i];
	  System.out.println("Rollnumber of " + i+"th student befor update is " +StdNum);
	  
  }
  for(int i=0;i<len;i++)
  {
	  numbers[i] = numbers[i] +i+1;
	 int StdNum = numbers[i];
	 System.out.println("Rollnumber of " + i+"th student after update is " +StdNum);
  }
  
}   
	@Test
	public void intArrayList()
	{
		ArrayList<Integer> numbers = new ArrayList<Integer>();
		//int[] numbers = {1,2,3,4,5,6,7};
		  int  len = numbers.size();
		  System.out.println("Lenght of array:" +len);
		  //int firstnum =numbers[0];
		  for(int i=0;i<len;i++)
		  {
			        int StdNum = numbers.get(i);
			  System.out.println("Rollnumber of " + i+"th student befor update is " +StdNum);
			  
		  }
		  for(int i=0;i<10;i++)
		  {
			  numbers.add(i+4);
			 int StdNum = numbers.get(i);
			 System.out.println("Rollnumber of " + i+"th student after update is " +StdNum);
		  }
		  System.out.println("Lenght of array after adding:" +numbers.size());
	}
}
