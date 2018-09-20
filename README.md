# StringManipulation1
Substring2
import java.util.Scanner;

public class substring2 {
    public static void main(String[] args) {
		
    	
    	//Ask user to enter a word. 
    	//If the first or second or both letter of the word is x, print the word without x
    	//(s).If x is the third letter it should be printed. If the first and second are x, both should be 
    	//ignored.
    	Scanner keyboard = new Scanner (System.in);
    	System.out.println("Enter please a word");
    	String word = keyboard.nextLine();
    	
    	if (word.charAt(0)=='x' && word.charAt(1)=='x') {
    		System.out.println(word.substring(2));
    	} else if (word.charAt(0)=='x') {
    		System.out.println(word.substring(1));
    	} else if (word.charAt(1)=='x') {
    		System.out.println(word.replace("x",""));
    	}
    		keyboard.close();
    	
	}
}
