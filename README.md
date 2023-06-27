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

Test: "It shoudl return 1 occurence of a word when the word and the text are the same."
Code:
const text = "red"
const word = "red"
numberOfOccurencesInText(word, text);
Expected Output: 1