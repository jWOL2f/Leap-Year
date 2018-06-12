# Leap-Year
//Figures out if the year you entered is a leap-year.

import java.util.Scanner;

public class Application {

	public static void main(String[] args) {

		// create scanner object
		Scanner input = new Scanner(System.in);
		// output the promt
		System.out.println("Please enter a Year: ");
		// wait for the user to enter something
		int value = input.nextInt();
		// tell them what they entered
		System.out.println("You entered the Year: " + value);

		boolean cond1 = value % 4 == 0;
		boolean cond2 = value % 100 == 0;
		boolean cond3 = value % 400 == 0;

		if (cond3 == true) {

			System.out.println("The Year " + value + " was/is a leap-year.");

		} else if (cond2 == true) {

			System.out.println("The Year " + value + " wasn't/isn't a leap-year!!!");

		} else if (cond1 == true) {

			System.out.println("The Year " + value + " was/is a leap-year.");

		} else {

			System.out.println("The Year " + value + " wasn't/isn't a leap-year!!!");
		}
	}
}
