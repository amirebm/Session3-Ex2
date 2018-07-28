# Session3-Ex2


// ب ن ک که عددی از ورودی دریافت کند و کامل بودن و یا نبودن آن را بررسی کند 

package com.persona.Ex2;

import java.util.Scanner;

public class Ex2 {

public static void main(String[] args) {
		
		Scanner sc= new Scanner(System.in);
		System.out.println("Enter a Number");
		int completeNum= sc.nextInt();
		if(CompleteFinder(completeNum)== completeNum )
			{System.out.println(completeNum + " is a Complete number");}
		else
			System.out.println(completeNum + " is not a Complete number");
			}
		
	
	
	static int CompleteFinder(int completeNum) {
		int sum=0;
		for (int i = 1; i < completeNum; i++) {
			
			if(completeNum %i==0) {
				sum+=i;
			}
			
			}
		return sum;
		
	}

}
  
