# work-code
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
        }
        System.out.print("\n\nThe sum is: " + sum);
        double avg = sum/age.length;
        System.out.println("\n\nThe avarage is: " + avg);
	}


}
//simple program in c language to input name and give an output

