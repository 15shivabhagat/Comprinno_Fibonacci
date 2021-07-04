# Comprinno_Fibonacci
package p2;
import java.util.Scanner;
public class Test {

	public static void main(String[] args) {
		  Scanner sc = new Scanner(System.in);
		 
		  System.out.println("Enter the Number of Test Cases");
		  //Initializing Test Cases for the Iteration
		    int t=sc.nextInt();
		  
		    sc.nextLine();
		  //Initializing String to check is it Dynamic or Not
		    String str = sc.nextLine();
		   //Converting String into Character Array 
		    char arr[]=str.toCharArray();
		    //It is used to store Fibonacci Condition result
		    int flag=0;
		    for(int i=2; i<t; i++) {
		    	 if(arr[i]+arr[i+1]==arr[i-2]+arr[i-1]) {
				    	flag =1;
				    }
		    	 else {
		    		 flag=0;
		    		 break;
		    	 }
		    }
		    if(flag==1) {
		    	System.out.println("Dynamic");
		    }
		    else {
		    	System.out.println("Not");
		    }
		   
		    
		  }
	}


