import java.util.Scanner;
public class BMI CALCULATOR{
	public static void main(String[] args) {
	
    	Scanner input = new Scanner(System.in);
		
		System.out.print("Enter your weight (kg): ");
		double weight = input.nextDouble();
		
		System.out.print("Enter your height (cm): ");
		double height = input.nextDouble();
		
		double bmi = (weight / (height * height));
		
		 
		
		String category;

        if (bmi < 18.5) {
            category = "Underweight";
        } else if (bmi >= 18.5 && bmi <= 24.9) {
            category = "Normal Weight";
        } else if (bmi >= 25 && bmi <= 29.9) {
            category = "Overweight";
        } else {
            category = "Obese";
        }


		
		System.out.println("=======Results======");
		System.out.println("Your weight (kg): " + weight);
		System.out.println("Your height (cm): " + height);
		System.out.println("Your BMI: " + bmi);
		System.out.println("Your health category: " + category);
		input.close();
	}
}
