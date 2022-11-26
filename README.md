# StringInputAfterInt
````
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        double d = sc.nextDouble();
        sc.nextLine();
        String st= sc.nextLine();
        
        System.out.println("String: "+st);
        System.out.println("Double: "+d);
        System.out.printf("Int: %d",n);
    }
}
````

After Inputing Integer/Double, the StringInput `nextLine()` skips our inputed String. \
This is a common problem, and it happens because the `nextInt()` method doesn't read the newline character of your input, \
so when you issue the command `nextLine()`, the `Scanner` finds the newline character and gives you that as a line.
