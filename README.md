
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter total subjects: ");
        int c = sc.nextInt();
        int [][] marks = new int[8][c];
        
        for(int i=0; i< 8; i++){
            System.out.println((i+1) + " Semester marks:- ");
            for(int j=0; j<c; j++){
                System.out.println("Enter " +(j+1)+ " Subject marks: ");
                int m = sc.nextInt();
                marks[i][j] = m;
                
                if( marks[i][j] > 100) {
                    System.out.print("Invalid marks! Enter in range of 100");
                    }
                else if( marks[i][j] >= 90 && marks[i][j] <= 100) {
                    System.out.print("Grade: A+ , Grade point: 4.0");
                    }
                else if( marks[i][j] >= 85 && marks[i][j] <= 89) {
                    System.out.print("Grade: A , Grade point: 4.0");
                    }
                 else if( marks[i][j] >= 80 && marks[i][j] <= 84) {
                    System.out.print("Grade: A- , Grade point: 3.8");
                    }
                 else if( marks[i][j] >= 75 && marks[i][j] <= 79) {
                    System.out.print("Grade: B+ , Grade point: 3.4");
                    }
                else if( marks[i][j] >= 71 && marks[i][j] <= 74) {
                    System.out.print("Grade: B, Grade point: 3.0");
                }
                else if( marks[i][j] >= 68 && marks[i][j] <= 70) {
                    System.out.print("Grade: B- , Grade point: 2.8");
                }
                else if( marks[i][j] >= 64 && marks[i][j] <= 67) {
                    System.out.print("Grade: C+ , Grade point: 2.4");
                }
                else if( marks[i][j] >= 61 && marks[i][j] <= 63) {
                    System.out.print("Grade: C, Grade point: 2.0");
                }
                else if( marks[i][j] >= 57 && marks[i][j] <= 60) {
                    System.out.print("Grade: C- , Grade point: 1.8");
                }
                else if( marks[i][j] >= 53 && marks[i][j] <= 56) {
                    System.out.print("Grade: D+ , Grade point: 1.4");
                }
                else if( marks[i][j] >= 50 && marks[i][j] <= 52) {
                    System.out.print("Grade: D, Grade point: 1.0");
                }
                else{
                    System.out.print("Fails, 0.0");
                }
                
            }
            System.out.println();
        }
    }
}
