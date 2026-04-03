# Repeated Questions

## ARMSTRONG NUMBER
```java
import java.util.*;

class Main {
    public static void main(String[] args) {
        
       int num=1634;
       
       String n=Integer.toString(num);
       
       int ans=0;
       
       for(char c:n.toCharArray())
       {
           ans+=(int)Math.pow(c-'0',n.length());
       }
       
       
        System.out.println(ans);
    }
}
```
## two consecutive vowels
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        String sentence = sc.nextLine();

        String[] words = sentence.split(" ");
        int count = 0;

        for(String word : words)
        {
            if(hasConsecutiveVowels(word))
            {
                count++;
            }
        }

        System.out.println(count);
    }

    public static boolean hasConsecutiveVowels(String word)
    {
        String vowels = "aeiouAEIOU";

        for(int i=0;i<word.length()-1;i++)
        {
            if(vowels.indexOf(word.charAt(i))!=-1 &&
               vowels.indexOf(word.charAt(i+1))!=-1)
            {
                return true;
            }
        }

        return false;
    }
}
```
## NUMBER REVERSE
```java
import java.util.*;
class Main {
    public static void main(String[] args) {
        
        int a=21547688;
        int temp=a;
        int dig=0;
        int count=0;
      
        while(temp!=0)
        {
            int rev=temp%10;
            dig=dig*10+rev;
            temp/=10;
               if(dig%2==0)
            {
                count++;
            }
            
        }
         System.out.print(dig);
    
    }
}
```
