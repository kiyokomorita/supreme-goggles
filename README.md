# Lab 1

## Q1: 
> Write a Java program with a method named 'totalSum' that takes in an argument of two integers and return its sum. Call this method from main( ) and print the results.

Answer :
public static int totalSum(int a, int b) {
		return a +b;
	}
	

	public static void main(String[] args) {
		int result = totalSum(2,3);
		
		System.out.println(result);
	}
## Q2:
> Write a Java program with a method named 'getGrades' that will display grades according to the marks entered into the method call as below:
```
Marks        Grade
91-100         A+
81-90          A-
71-80          B+
61-70          B-
51-60          C+
41-50          D-
<=40          Fail
```
Answer:

public static void getGrades (int grade) {
		
		if (grade >90 && grade <=100) {
			System.out.println ("A+");
	
	}else if(grade >=81 && grade <=90){
			System.out.println ("A-");
	
	}else if(grade >=71 && grade <=80) {
		System.out.println ("B+");
}else if(grade >=61 && grade <=70){
	System.out.println ("B-");
}else if(grade >=51 && grade <=60){
	System.out.println ("C+");
}else if(grade >=41 && grade <=50){
	System.out.println ("D-");
}else if (grade <=40) {
	System.out.println("Fail");
}else {
	System.out.println("error");
}
	}

	public static void main(String[] args) {
		getGrades(95);

	}

## Q3:
> Write a program to print the factorial of a number by defining a method named 'factorial'. Factorial of any number n is represented by n! and is equal to 1*2*3*....
``` 
4! = 1*2*3*4 = 24
3! = 3*2*1 = 6
2! = 2*1 = 2
Also,
1! = 1
0! = 0
```
Answer:
	public static void factorial(int n) {
		int result = 1;
		if (n==0) {
			result = 0;
		
	
		}else {
			for (int i=1; i<=n; i++) {
				 result=result*i;
			 
		 }
		}
		System.out.println(result);
	}

	public static void main(String[] args) {
      factorial(5);

}
## Q4
> Write a Java method to create the area of a pentagon.

Answer is
public static double areaofpentagon(double side, double length) {
		return ((double)(5/2)*side * length);
		
		
	}

	public static void main(String[] args) {

		double result = areaofpentagon(5.7,4.0);
		System.out.println(result);
		

	}

