# competitive-java-problems
i love java
package com.company;

import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

public class vvvimp {
    public static void main(String[] args) {
        int flag = 0;
     
Scanner sc=new Scanner(System.in);
int n=sc.nextInt();
int a[]={3,5,7};



        List<Integer> fac=new ArrayList<Integer>();
        while(flag<=n){
            for (int i = 1; i < 100; i++) {

                for (int j = 0; j < a.length; j++) {
                    if (i % a[j] == 0) {
                        //  System.out.print(i + ",");
                        flag=flag+1;

                        for(int k=flag;k<=n;k++){
                            fac.add(i);
                            break;
                        }
                        break;



                    }
                }

            }
        }
        for (int ans:fac) {
            System.out.print(ans+" ");


        }
    }
}
