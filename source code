import javax.swing.*;
 
public class NumberGuessGame{
    public static void main(String[] args) {
        int RandomNumber = (int) (Math.random()*100 + 1);
        int GuessingNumber = 0;
        int count = 1;
        System.out.println(RandomNumber);

        while (GuessingNumber != RandomNumber)
        {
            String response = JOptionPane.showInputDialog(null,
                "Enter a guess between 1 and 100", "Guessing Game", 3);
            GuessingNumber = Integer.parseInt(response);
            JOptionPane.showMessageDialog(null, ""+ determineGuess(GuessingNumber, RandomNumber, count));
            count++;
        }  
    }

    public static String determineGuess(int userAnswer, int computerNumber, int count){
        if (userAnswer <=0 || userAnswer >100) {
            return "Your guess is invalid";
        }
        else if (userAnswer == computerNumber ){
            return "You got it!\nTotal Guesses: " + count;
        }
        else if (userAnswer > computerNumber) {
            if(userAnswer-10<=computerNumber){
                return "You are very near,your guess is not too high,try again.\nTry Number:" + count;
            }
            return "Your guess is too high, try again.\nTry Number: " + count;
        }
        
        else if (userAnswer < computerNumber) {
            if(userAnswer+10>=computerNumber){
                return "You are very near,your guess is not too low,try again.\nTry Number:" +count;
            }
            return "Your guess is too low, try again.\nTry Number: " + count;
        }
        else {
            return "Your guess is incorrect\nTry Number: " + count;
        }
    }}
   
