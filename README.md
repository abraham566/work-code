import java.util.ArrayList;
import java.util.Scanner;

public class TaskManager {
    public static void main(String[] args) {
        ArrayList<String> tasks = new ArrayList<>();
        Scanner scanner = new Scanner(System.in);

        while (true) {
            System.out.println("Choose an option:");
            System.out.println("1. Add task");
            System.out.println("2. Mark task as completed");
            System.out.println("3. View to-do list");
            System.out.println("4. Exit");

            int choice = scanner.nextInt();
            scanner.nextLine(); // Consume newline

            switch (choice) {
                case 1:
                    System.out.print("Enter task: ");
                    String task = scanner.nextLine();
                    tasks.add(task);
                    System.out.println("Task added!");
                    break;
                case 2:
                    System.out.print("Enter task index to mark as completed: ");
                    int index = scanner.nextInt();
                    if (index >= 0 && index < tasks.size()) {
                        tasks.remove(index);
                        System.out.println("Task marked as completed!");
                    } else {
                        System.out.println("Invalid index.");
                    }
                    break;
                case 3:
                    System.out.println("To-do list:");
                    for (int i = 0; i < tasks.size(); i++) {
                        System.out.println(i + ". " + tasks.get(i));
                    }
                    break;
                case 4:
                    System.out.println("Exiting. Have a great day!");
                    return;
                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }
}# work-code
code hacks
[Uploading p
    
    public class Mate {
    
        
    
     public static void main(String[] args) {
          int time = 2;
          if (time < 18) {
            System.out.println("name.");
          } else {
            System.out.println("marks.");
          }  
        }
      }
    import java.util.*;

public class Reallife {

	public static void main(String[] args) {
		
		int age[] = {20,23,19,18,17,19,19,18,21,24,26,24,19,18,18,19};
		
		System.out.println(age.length);
		int max = Arrays.stream(age).max().getAsInt();
		System.out.println(max);
		Arrays.sort(age); // Sorts the array in ascending order
        for (int i : age) {
            System.out.print(i + " ");
            
        }
        
        int sum = 0;
        for (int i = 0; i < age.length; i++) {
            sum += age[i];

        System.out.print("\n\nThe sum is: " + sum);
        double avg = sum/age.length;
        System.out.println("\n\nThe avarage is: " + avg);
	}


}
//simple program in c language to input name and give an output
![WhatsApp Image 2024-07-03 at 09 54 40_745e1755](https://github.com/abraham566/work-code/assets/172487457/721aeb61-873b-4e52-99b5-8f26c280d8d6)
[16/07/2024 10:52 AM] : //Java program to display today`s date
//import date
import java.util.Date;
public class date{
 public static void main(String args[]) {
 //main class
 Date d = new Date();
 //Display time and date using toString{}
 System.out.println(d.toString());

 }
}
[16/07/2024 10:53 AM] : r;
import java.util.Formatter;

public class MainClass{
   public static void main(String args[]) {
      Formatter fmt = new Formatter();
      Calendar cal = Calendar.getInstance();
      fmt = new Formatter();
      fmt.format("%tc", cal);
      System.out.println(fmt);
   }
}
[16/07/2024 11:11 AM] : import java.time.LocalDate;
import java.time.Period;
import java.util.Scanner;

public class AgeCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input birthdate (format: yyyy-MM-dd)
        System.out.print("Enter your birthdate (yyyy-MM-dd): ");
        String birthdateStr = scanner.nextLine();
        LocalDate birthdate = LocalDate.parse(birthdateStr);

        // Current date
        LocalDate currentDate = LocalDate.now();

        // Calculate age
        int age = calculateAge(birthdate, currentDate);

        // Output age
        System.out.println("Your age is: " + age + " years");
    }

    public static int calculateAge(LocalDate birthdate, LocalDate currentDate) {
        return Period.between(birthdate, currentDate).getYears();
    }
}
[16/07/2024 11:57 AM] droidRAZR: // imports
import java.util.*;
import java.time.*;

//main Class

public class date{

//main method
		 public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        
        LocalDate currentDate = LocalDate.now();
        System.out.print("Enter year :");
        int year = scanner.nextInt();
        System.out.print("Enter month:  ");
        int month = scanner.nextInt();
        System.out.print("Enter day : ");
        int day = scanner.nextInt();


        LocalDate inputDate = LocalDate.of(year, month, day);

       
        Period period = Period.between(inputDate, currentDate);

       
        System.out.print("Yours is" +period.getYears());

        scanner.close();
		}
}
