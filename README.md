# Random-Code

/*******************************************************************************
*                     Assignment 1 -- Information and Instructions             *
*                                                                              *
* PROGRAMMER:        Caden Bonnell, bonn6558@unco.edu                          *
* CLASS:             CS160 -- Structured Programming                           *
* INSTRUCTOR:        Dean Zeller                                               *
* TERM:              Fall 2020                                                 *
* SUBMISSION DATE:   9/4/20                                                    *
*                                                                              *
* DESCRIPTION:                                                                 *
* Use input and print to create a program that will tell you the addition of 3 *
* inputed numbers, as well as take the average of those three numbers.         *
*                                                                              *
* COPYRIGHT:                                                                   *
* This program is copyright (c)2020 Caden Bonnell and Dean Zeller.             *
* It is original work without use of outside sources.                          *
*                                                                              *
*******************************************************************************/


/* 
Information and Instructions
This section of code gathers the user's name and name of the study,
and informs the user of what this program will accomplish. 
*/

import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
    Scanner scnr = new Scanner(System.in);

      int firstNum;
      int secondNum;
      int thirdNum;
      int totalNum;
      int averageNum;
      String userName;
      String studyName;
      
      
      System.out.println("Please enter your name => ");
      userName = scnr.next();
      System.out.println("Hello " + userName);
        
      System.out.println("Please enter the title of the study => ");
      studyName = scnr.next();
      System.out.println("Study title set to " + studyName);
      
      
      System.out.println("Introduction:");
      System.out.println("This process will calculate basic statistics on three");
      System.out.println("ineger numbers.  It will run in three phases:");
      System.out.println("    Phase 1 - Gather data from user ");
      System.out.println("    Phase 2 - Perform calculations ");
      System.out.println("    Phase 3 - Output results ");
      System.out.println("");
    
/* 
PHASE 1 - GATHER DATA
This phase gathers the neccessary input from the user. 
Three integer values are read. 
*/
    
      System.out.println("Phase 1: Gather data from user");
      System.out.println("------------------------------");
      System.out.println("Please enter three numbers. Only enter integer values,");
      System.out.println("as error-checking has not yet been implemented.");
    
      System.out.println("    First number => ");
      firstNum = scnr.nextInt();
      
      System.out.println("    Second number => ");
      secondNum = scnr.nextInt();
      
      System.out.println("    Third number => ");
      thirdNum = scnr.nextInt();
      
      System.out.println("Numbers entered: " + firstNum + " " + secondNum + " " + thirdNum);
      System.out.println("Phase 1 complete");
      System.out.println("");
          
      totalNum = firstNum + secondNum + thirdNum;
      averageNum = (firstNum + secondNum + thirdNum) / 3;
      
 /* 
PHASE 2 - PERFORM CALCULATIONS 
This section of code performs the neccesary calculations ,
including calculating the total and the average of the input
entered in Phase 1.
*/
      
      System.out.println("Phase 2: Perform calculations");
      System.out.println("-----------------------------");
      System.out.println("    Calculated total (" + totalNum + ")");
      System.out.println("    Calculated average (" + averageNum + ")");
      System.out.println("Phase 2 complete");
      System.out.println("");
      
  
/* 
PHASE 3 - ENTER RESULTS 
This phase creates a report for the output.
*/  
      
      System.out.println("Phase 3: Output results");
      System.out.println("-----------------------");
      System.out.println("");
      System.out.println("Study:        " + studyName);
      System.out.println("Researcher:   " + userName);
      System.out.println("Data:         " + firstNum + " " + secondNum + " " + thirdNum);
      System.out.println("Total:        " + totalNum);
      System.out.println("Average:      " + averageNum);
      
      System.out.println("");
      System.out.println("Phase 3 complete");
      System.out.println("");
      System.out.println("Exiting Program");
      
      
  }
}

