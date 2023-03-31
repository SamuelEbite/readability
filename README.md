# readability

This Python script takes in a text input from the user, counts the number of letters, words, and sentences in the text, and then calculates the Coleman-Liau index for the text. The Coleman-Liau index is a readability test designed to gauge the readability of a text.

Requirements
This script uses the cs50 module. If you don't have this module installed on your machine, you can install it using the command:

Copy code
pip install cs50
Usage
To use the script, simply run it from the command line and follow the prompts. The script will ask you to input a text and will then print out the grade level of the text according to the Coleman-Liau index.

How it Works
The script first prompts the user to input a text using the get_string function from the cs50 module. It then initializes variables to count the number of letters, words, and sentences in the text.

The script then loops through each character in the text and counts the number of letters, words, and sentences based on certain conditions. Once it has counted these values, it calculates the Coleman-Liau index using the formula:

bash
Copy code
index = 0.0588 * (letter/words*100) - 0.296 * (sentences/words*100) - 15.8
The script then prints out the grade level of the text according to the Coleman-Liau index. If the index is less than 1, the text is considered to be at a pre-kindergarten reading level. If the index is greater than or equal to 16, the text is considered to be at a college graduate reading level.
