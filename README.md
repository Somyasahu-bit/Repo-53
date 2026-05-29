# Repo-53
Check whether given number is Prime or not
import java.util.*;
 public class Third {
    public static boolean isPrime (int num) {
        int cnt=0;
        if (num <=1 ){
            return false;
        }
        for(int i = 2; i * i <= num; i++) {
            if (num % i == 0) {
                return false;
            }
        }
        return true;
    }
    public static void main (String args[]) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        if (isPrime(num)) {
            System.out.print("yes its a prime number");
        }else {
            System.out.print("no its not a prime number");
        }
        sc.close();
    }
 }
