# COP2334-1-Module-8-Assignment
This is a GitHub repository link for the C++ Programming Assignment from Module 8.

// This program is used to count the number of characters in a string like a sentence, a paragraph, or a word.

// inclusion of iostream and string library
#include <iostream>
#include <string>
using namespace std; // using standard namespace

// function for counting the number of characters in a string.
int countChars(char *str);

// main function
int main() {
  char str[100]; // declaring a character array of size 100.
  const int SIZE = 101; // declaring a constant integer of size 100.
  cout << "Enter a string with 100 characters or less: \n"; // prompting the user to enter a string.
  cin.getline(str, SIZE); // reading the string from the user.
  cout << "The number of characters in the string is: " << countChars(str) << endl; // printing the number of characters in the string.
  return 0; // returning 0 to the main function.
}

int countChars(char *str) { // function for counting the number of characters in a string.
  int count = 0; // declaring an integer variable count and initializing it to 0.
  while (*str != '\0') { // while loop to iterate through the string until the end of the string is reached.
    count++; // incrementing the count variable by 1.
    str++; // incrementing the pointer to the next character in the string.
  }
  return count; // returning the count variable to the main function.
}
