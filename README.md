# reversing-array
import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.regex.*;


public class Solution {
    public static void main(String[] args){
        Scanner scan=new Scanner(System.in);
        int N=scan.nextInt();
                int arr[]=new int [N];

        for(int i=0;i<N;i++){
            arr[i]=scan.nextInt();
            
        }
        
        for(int i=0;i<=(N-1)/2;i++){
            int temp=arr[i];
            arr[i]=arr[N-1-i];
            arr[N-1-i]=temp;
        }
        
        for(int i=0;i<N;i++){
            System.out.print(arr[i]+" ");
        }
    }
}
