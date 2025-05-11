import java.util.*;

 public class Cutoff_Calculator {
	
	public static void main (String[]args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Welcome to Calculator 12th cutoff");
		boolean calculatorAgain = true;
	
		while(calculatorAgain) {
				System.out.println("Medical Cutoff (Press 1) or Engineering Cutoff(Press 2)");
				int syb = sc.nextInt();
				if(syb==1) {
					double Biology = getvalidmark(sc,"Biology");
					double Physics = getvalidmark(sc,"Physics");
					double Chemistry = getvalidmark(sc,"Chemistry");
				    double  pc = Physics+Chemistry;
				    double  cutoff= Biology+(pc/2);
				    System.out.println("Cutoff Medical "+ cutoff);
				}
				else if(syb==2){
					double Maths = getvalidmark(sc,"Maths");
					double Physics = getvalidmark(sc,"Physics");
					double Chemistry = getvalidmark(sc,"Chemistry");
					double pc = Physics+Chemistry;
					double cutoff= Maths+(pc/2);
					System.out.println("Cutoff Engineering "+ cutoff);
					
				}
				System.out.println("Do you want to calculate again(yes/no)");
				sc.nextLine();
				String again =sc.nextLine();
				if(again.equalsIgnoreCase("NO")) {
					 calculatorAgain = false;
					 System.out.println("\tTHANK YOU");
				}
				
			}
		
		}
	
	
	public static double getvalidmark(Scanner sc,String Subject) {
	double mark;
	while(true) {
		System.out.println("Enter "+Subject+" Marks(0-100) ");
		mark =sc.nextDouble();
		if(mark>=0 && mark<=100) {
			break;
		}
		else {
			System.out.println("Invalid Mark! Please Enter Between 0 and 100.");
		}
	}
	return mark;
}
 }
