# DATA-COMPRESSION-TOOL

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RAVI PRABHA

*INTERN ID*: CT04DN1602

*DOMAIN*: C PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

## (The provided C program implements Run-Length Encoding (RLE), a basic form of data compression used to reduce the size of a string by replacing consecutive repeated characters with a single character followed by the number of repetitions. This method is especially useful for strings containing many repeated characters, such as "aaabbbcccc" being compressed to "a3b3c4".

Program Overview

The program starts with including the necessary header files: stdio.h for standard input-output operations and string.h for string manipulation functions. The key function in the code is runLengthEncode(), which performs the actual compression logic.

main() Function

The execution begins in the main() function where:

1. A character array input of size 100 is declared to store the user's input string.


2. The program prompts the user to enter a string (without spaces).


3. It reads the string using scanf() and then calls runLengthEncode() with the input as an argument.


4. The compressed result is printed to the console.



runLengthEncode() Function

This function is responsible for compressing the string. It performs the following steps:

1. Initialization:
It calculates the length of the string using strlen() and initializes a count variable to keep track of character repetitions.


2. Character Traversal:
It uses a for loop to iterate over each character in the string.


3. Counting Repeats:
Inside the loop, it compares each character with the next one (input[i] == input[i + 1]). If they match, it increases the count and increments i to move to the next character. This continues as long as the current character equals the next one and the index is within bounds.


4. Output:
Once a different character is found or the end of the string is reached, it prints the current character followed by its count, such as "a3".


5. Loop Continuation:
The process repeats for the entire string until all characters are processed.


6. Newline:
After compression is complete, a newline is printed for output formatting.



Example Execution

If the input is:

aaabbcddd

The output will be:

a3b2c1d3

Each character is followed by the number of times it appears consecutively.

Notes and Considerations

This program assumes no spaces in the input, as scanf("%s", input) reads up to the first whitespace.

It handles only basic run-length encoding; it does not handle decoding.

If the string contains many different characters in sequence (like "abcdef"), compression may not be effective as each character will be followed by 1.


Use Cases

Run-length encoding is used in:

Image compression formats like TIFF and BMP.

Basic text compression.

Situations where storage or transmission of repeated data needs optimization.


Overall, the program serves as a simple and effective demonstration of how RLE works using basic C programming constructs.)

#OUTPUT
![Image](https://github.com/user-attachments/assets/416c4a5e-53c5-4479-885e-46a91efa00af)
