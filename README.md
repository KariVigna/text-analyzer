Describe: wordCounter()

Test: "It should return 1 if a passage has just one word."
Code:
const text = "hello";
wordCounter(text);
Expected Output:1

Test: "It should return 2 if a passage has 2 words."
Code:
const text = "hello there";
wordCounter(text);
Expected Output: 2

Test: "It should return 0 for an empty string."
Code: wordCounter("");
Expected Output: 0;

Test: "It should return 0 for a string that is only spaces."
Code: wordCounter("   ");
Expected Output: 0;

Test: "It should not count numbers as words."
Code: wordCounter("hi there 77 19");
Expected Output: 2;


Describe: numberOfOccurencesInText(word, text);

Test: "It should return 0 occurences of a word for an empty string."
Code:
const text = "";
const word = "red";
numberOfOccurencesInText(word, text);
Expected Output: 0;

Test: "It should return 1 occurence of a word when the word and the text are the same."
Code:
const text = "red"
const word = "red"
numberOfOccurencesInText(word, text);
Expected Output: 1

Test: "It should return 0 occurences of a word when the word and the text are different."
Code:
const text = "red";
const text = "blue";
numberOfOccurencesInText(word, text);
Expected Output: 0

Test: "It should return the number of occurences of a word."
const text = "red blue red red red green";
const word = "red";
numberOfOccurencesInText(word, text);
Expected Output: 4

Test: "It should return a word match regardless of case."
Code:
const text = "red RED Red green Green GREEN";
const word = "Red";
numberOfOccurencesInText(word, text);
Expected Output: 3

Test: "It should return a word match regardless of punctuation."
Code:
const text = "Red! Red. I like red, green, and yellow.";
const word = "Red";
numberOfOccurencesInText(word, text);
Expected Output: 3


Describe: wordCheck();
Test: "It should return 'No thank you' for offensive words"
Code:
const text = "zoinks red green"
const word