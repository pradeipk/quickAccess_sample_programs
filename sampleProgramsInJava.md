# Sample Programs in Java 

## Contents
[Reverse a string](Reverse-a-string)


## Reverse a string

```sh
public class StringPrograms {

    public static void main(String[] args) {

        String str = "123";
        System.out.println(reverse(str));
    }

    public static String reverse(String in) {
        if (in == null)
            throw new IllegalArgumentException("Null is not valid input");

        StringBuilder out = new StringBuilder();

        char[] chars = in.toCharArray();

        for (int i = chars.length - 1; i >= 0; i--)
            out.append(chars[i]);

        return out.toString();
    }
}

```
## Java Program to check if a vowel is present in the string?

```sh
public class StringContainsVowels {

    public static void main(String[] args) {

        System.out.println(stringContainsVowels("Hello")); // true
        System.out.println(stringContainsVowels("TV")); // false

    }

    public static boolean stringContainsVowels(String input) {

        return input.toLowerCase().matches(".*[aeiou].*");

    }

}

```


## Palindrome 
```sh
boolean checkPalindromeString(String input) {
    boolean result = true;
    int length = input.length();
    for(int i=0; i < length/2; i++) {
        if(input.charAt(i) != input.charAt(length-i-1)) {
            result = false;
            break;
        }
    }
    return result;
}
```

## Based on Java 8 Features




