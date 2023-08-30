
package studentgrade;
import java.util.Scanner;


public class StudentGrade {

    
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("How many subject you have ??? ");
        int n =sc.nextInt();
        System.out.println("Enter the subject marks out of 100 :--");
        int i=0,t=0;
        while(i<n){
            int a =sc.nextInt();
            t=t+a;
            i++;
        }
        double avg_per = t/n;
        String gd ;
        if(avg_per>=80 && avg_per<200){
           gd ="AA";
        }
       else if(avg_per>=70 && avg_per<80){
            gd ="AB";
        }
       else if(avg_per>=60 && avg_per<70){
             gd ="BB";
        }
       else if(avg_per>=55 && avg_per<60){
             gd ="BC";
        }
         else if(avg_per>=50 && avg_per<55){
              gd ="CC";
        }
         else if(avg_per>=45 && avg_per<50){
             gd ="CD";
        }
         else if(avg_per>=40 && avg_per<45){
            gd ="DD";
        }
         else if(avg_per>=00 && avg_per<40){
           gd ="FF";
        }
        else{
             gd = " absent in examination";
        }
        
         System.out.println("Total Marks" + "     " +  "Average Percentage"  + "      " +  "Grade ");
         System.out.println(       (t)  +"            " +   (avg_per)   +"                     " + gd  );
        
    }
    
}
