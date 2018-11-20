package com.app;
import java.util.Arrays; 
public class SortedList
{ 
	public static void alternateSort(int arr[], int n) 
    { 
        Arrays.sort(arr); 
        int i = 0, j = n-1; 
        while (i < j) { 
            System.out.print(arr[j--] + " "); 
            System.out.print(arr[i++] + " "); 
        } 
       if (n % 2 != 0) 
    	   System.out.print(arr[i]); 
    } 
  
   
    public static void main (String[] args) 
    { 
        int arr[] = {4, 5, 7, 7, 6, 5, 4, 3}; 
        int n = arr.length; 
        alternateSort(arr, n); 
    } 
} 
