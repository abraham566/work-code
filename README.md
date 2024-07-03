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
