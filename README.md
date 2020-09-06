# EnrollmentSystem

package enrollment.system;

import java.util.Scanner;

public class EnrollmentSystem {

  
    public static void main(String[] args) {
       String firstName, midName, lastName, studAdress, studPrevSchl,studGuardian, guarNo, yearGrad, strand;

       char secMawd = 'A';
       char secHumss = 'A';
       char secRbo = 'A';
       char secCulArt = 'A';
       char secTro = 'A';
       
       String select = "MAWD";
       String select2 = "HUMSS";
       String select3 = "RBO";
       String select4 = "CULART";
       String select5 = "TRO";
       
       
       int ctrMawd = 0;
       int ctrHumss = 0;
       int ctrRbo = 0;
       int ctrCulArt = 0;
       int ctrTro = 0;
       
     
       
       
       Scanner scan = new Scanner(System.in);
        for (int i = 0; i < 30; i++) {
            
           
        
       System.out.println("Enter Your Last Name: ");
       lastName = scan.nextLine();
       
       System.out.println("Enter Your First Name: ");
       firstName = scan.nextLine();
       
       System.out.println("Enter Your Middle Name: ");
       midName = scan.nextLine();
       
       System.out.println("Enter Your Adress: ");
       studAdress = scan.nextLine();
       
       System.out.println("Enter Your Previous Shool: ");
       studPrevSchl = scan.nextLine();
       
       System.out.println("Year Graduated: ");
       yearGrad = scan.nextLine();
       
       System.out.println("Enter your Guardian's Name: ");
       studGuardian = scan.nextLine();
       
       System.out.println("Enter YOur Guardian's Contact No: ");
       guarNo = scan.nextLine();
       
       System.out.println("Choose Your Strand Among The Following:" );
       
       System.out.println("NOTE: PLEASE USE ALL CAPS");
       
       System.out.println(" MAWD " + " HUMSS " + "RBO " + " CULART " + " TRO ");
       strand = scan.nextLine();
       
      if(strand .equals(select)){
          
        ctrMawd++;
          if(ctrMawd % 11 == 0){
              
              
              ++secMawd;
          }
          
      }
      
      
      if (strand .equals(select2)){
         ctrHumss++;
          
        if(ctrHumss % 11 == 0){
           
            ++secHumss;
          
           
        }
      }       
       if (strand  .equals(select3)){
         ctrRbo++;
          
        if(ctrRbo % 11 == 0){
           
            ++secRbo;
          
           
        }
      }     
        if (strand  .equals(select4)){
         ctrHumss++;
          
        if(ctrCulArt % 11 == 0){
           
            ++secCulArt;
          
           
        }
      }     
        if (strand  .equals(select5)){
         ctrTro++;
          
        if(ctrTro % 11 == 0){
           
            ++secTro;
          
           
        }
      }       
       
      
       System.out.println("Have you submitted your form 138: ");
       String sub = scan.nextLine();
       
       if ( sub .equals("yes") ){
       }
       else{
           System.out.println("You cannot proceed");
           System.exit(0);
       }
       
       
           System.out.println("Have you submitted your form 137: ");
           String rec = scan.nextLine();
           
                 if(rec .equals("yes")){
       
                 }
                 
              
                 
            System.out.println("Have You Submitted Your PSA Birth Certificate: ");
            String psa= scan.nextLine();
                     
            if(psa .equals("yes")){
                          
            }
            else{
                System.out.println("You cannot proceed without this document: ");
                System.exit(0);
            }
            
             System.out.println("Have You Submitted Your Good Moral: ");
             String goodMor=scan.nextLine();
                            
             if(goodMor .equals("yes")){
                                    
                                    
             }
             else{
                  System.out.println("You cannot proceed without this document: ");
                System.exit(0);
             }
             
             System.out.println(" Congratulation! " + firstName + " Welcome to STI! You are officialy enrolled in this school year 2020-2021 " );
             
             
             System.out.println("-----------------------------------------------------------------------------------------------------------------");
                 
             
             
             System.out.println(" DETAILS ");
             
             System.out.println("Last Name: " + lastName + " , " + "First Name: " + firstName + " , " + " Middle Name: " + midName );
             
             if (strand .equals(select))
             {
             System.out.println("Section: " + strand + "-1" + secMawd );
             
             } else if (strand .equals(select2)){
                 
                 System.out.println("Section: " + strand + "-1" + secHumss );
             }
             else if (strand .equals(select3)){
                 
                 System.out.println("Section: " + strand + "-1" + secRbo );
                
             }
             else if (strand .equals(select4)){
                 
                 System.out.println("Section: " + strand + "-1" + secCulArt );
                 
             }
             else if (strand .equals(select5)){
                 
                 System.out.println("Section: " + strand + "-1" + secTro );
             }
             
             System.out.println("Adress: " + studAdress);
             System.out.println("Previous School: " + studPrevSchl);
             System.out.println("Year Gradutaed in JHS: " + yearGrad);
             System.out.println("Guardian's Name: " + studGuardian);
             System.out.println("Guardian's Contact No:  " +  guarNo);
             if (rec .equals("yes")){
                    
                }
             else{
                System.out.println("Please submit Form 137 in the Office");
                }
                
             
             System.out.println("-----------------------------------------------------------------------------------------------------------------------------------------");
             
             System.out.println("Is there another enrolle: ");
             String stud= scan.nextLine();   
             
             if(stud .equals ("yes")){
                    
                }
             else{
                 System.exit(0);
             }
             
       }     
    }

    
    
}
