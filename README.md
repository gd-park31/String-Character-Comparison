# String Validation and Analysis Program

This Java project prompts the user to enter a string with **at least 12 characters**. 
It also checks if the string contains the characters `'a'`, `'e'`, and `'z'`. 

- If the string is shorter than 12 characters, it counts as an invalid attempt. 
  The user can only make **3 such attempts** before the program exits.
- If the string is 12+ characters but **missing** any of the required characters (`'a'`, `'e'`, `'z'`), 
  the user is prompted again without increasing the attempt count.
- Once a valid string is entered, the program **analyzes** it by counting:
  - **Uppercase letters**
  - **Lowercase letters**
  - **Digits**
  - **Special characters**

The program then displays the results and exits.

## Features
- **Length Validation**: Ensures the string is 12 or more characters long.
- **Character Presence**: Checks for the letters `'a'`, `'e'`, and `'z'`.
- **Three-Strike System**: Allows up to 3 invalid attempts for too-short inputs.
- **String Analysis**: Counts uppercase, lowercase, digits, and special characters.

## Example Run
Welcome to the String Validation Program!
Enter a string (>= 12 chars, containing 'a', 'e', 'z'): short
String is too short. Attempts used: 1 / 3
Enter a string (>= 12 chars, containing 'a', 'e', 'z'): abcdefghijk
String does not contain all required characters ('a', 'e', 'z').
Enter a string (>= 12 chars, containing 'a', 'e', 'z'): abcdefghijkz
String does not contain all required characters ('a', 'e', 'z').
Enter a string (>= 12 chars, containing 'a', 'e', 'z'): abCdefghijkz
String does not contain all required characters ('a', 'e', 'z').
Enter a string (>= 12 chars, containing 'a', 'e', 'z'): abcdeZfghijkz
Valid string received!

--- Analysis Results ---
String: abcdeZfghijkz
Uppercase letters:   1
Lowercase letters:   12
Digits:              0
Special characters:  0
