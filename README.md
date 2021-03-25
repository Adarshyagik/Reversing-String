# Reversing-String
Concating Two String And Reversing It
import java.util.*;
import java.io.*;
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
class MyClass {
    public static void main(String args[]) throws IOException {
        BufferedReader read =
            new BufferedReader(new InputStreamReader(System.in));
        int t = Integer.parseInt(read.readLine());
        while (t-- > 0) {
            String S1 = read.readLine();
            String S2 = read.readLine();
            Solution ob = new Solution();

            System.out.println(ob.conRevstr(S1, S2));
        }
    }
}

class Solution {
    static String conRevstr(String S1, String S2) {
       
        String str = new String();
        str = S1 + S2;
        String str1 = new String();
        
        for (int i = str.length() - 1; i >= 0; i--) {
            str1 += str.charAt(i);
        }
        return str1;
    }
}
