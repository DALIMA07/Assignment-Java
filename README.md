"# Assignment-Java" 

//Assignment 1: 

import java.util.*;


class GradeCalculator {
    
    public static void main(String[] args) {
        System.out.println("Enter Test Score : ");
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        if(n>100 || n<0){
            System.out.println("Grade is invalid");
        }
        else if(n>=90 && n<=100){
            System.out.println("Grade : A");
        }
        else if(n>=80 && n<=89){
            System.out.println("Grade : B");
        }
        else if(n>=70 && n<=79){
            System.out.println("Grade : C");
        }
        else if(n>=60 && n<=69){
            System.out.println("Grade : D");
        }
        else if(n>=50 && n<=59){
            System.out.println("Grade : E");
        }
        else{
            System.out.println("Grade : F");
        }
    }
}


// Assignment 2:


import java.util.*;

class MaxNumber {
    
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of array : ");
        int n = sc.nextInt();
        int max = 0;
        int index = 0;
        int[] arr = new int[n];
        System.out.println("Enter the values of the array elements : ");
        for(int i=0; i<n;i++){
            arr[i] = sc.nextInt();
        }
        
        for(int i=0; i<n;i++){
            if(arr[i]>max){
                max = arr[i];
                index = i+1;
            } 
            if(i==n-1){
                System.out.println("Maximum Number : " + max);
                System.out.println("Position of First Occurence : " + index);
            }
        }
    }
}
