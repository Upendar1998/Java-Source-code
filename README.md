# Java-Source-code
//Arm Strong Number
      

import java.util.Scanner;

public class Armstrong_Number {
public static void main(String args[]) {
	//Use scanner class 
	Scanner sc=new Scanner(System.in);
	System.out.println("Enter the Integer value");
	
	int number=sc.nextInt(),arm=0,rem,copy=number;
	
	while(number>0) {
		
	    rem=number%10;
	    
	    arm=arm+rem*rem*rem;
	    
	    number=number/10;
	}
	if(arm==copy) {
		System.out.println(copy+" Is a armstrong number");
	}
	else {
		System.out.println(copy+" Is not a armstrong number");
	}
}
}
