# Practical-rng
package com.discord.com.discord.maven.eclipse;

import java.util.Random;

public class Rng {
	
	public static void main(String args) {
		
	Random rnum = new Random(); //random object
	int i; //current count
	int[] numbers = new int[ 500]; //size 500
	numbers[0] = rnum.nextInt(1000); //first number initialize also declaring numbers array
	int large = numbers[0];
	int small = numbers[0];
	for (i=1 ; i < 500; i++) {
		numbers[i ] = rnum.nextInt(1000); //store numbers
		large = Math.max( large , numbers[i ] );
		small = Math.min(small, numbers[i ] );
	}
}
	
	
	


	}
