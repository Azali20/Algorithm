Initialize three variables as counters: "length" = 0, "words" = 1, "vowels" = 0.
Ask the user to input a sentence that ends with a point.
Loop through each character in the sentence:
a. Increment "length" by 1.
b. If the character is a space, increment "words" by 1.
c. If the character is a vowel (i.e., "a", "e", "i", "o", or "u"), increment "vowels" by 1.
Print out the results:
a. The length of the sentence is stored in the "length" variable.
b. The number of words in the sentence is stored in the "words" variable.
c. The number of vowels in the sentence is stored in the "vowels" variable.



For each character:
a. Increment the length counter.
b. If the character is a vowel (i.e., 'a', 'e', 'i', 'o', or 'u'), increment the vowelCount counter.
c. If the character is a space, increment the wordCount counter.


const sentence = "The quick brown fox jumps over the lazy dog.";
for (let i = 0; i < sentence.length; i++) {
  const char = sentence.charAt(i);
  if (char === '.') {
    break; // exit loop when the point is reached
  }
  length++; // increment length counter
  if ('aeiou'.includes(char.toLowerCase())) {
    vowelCount++; // increment vowel counter
  }
  if (char === ' ') {
    wordCount++; // increment word counter
  }
}
If the last character is not a space, increment the wordCount counter.
csharp
Copy code
const sentence = "The quick brown fox jumps over the lazy dog.";
for (let i = 0; i < sentence.length; i++) {
  const char = sentence.charAt(i);
  if (char === '.') {
    break; // exit loop when the point is reached
  }
  length++; // increment length counter
  if ('aeiou'.includes(char.toLowerCase())) {
    vowelCount++; // increment vowel counter
  }
  if (char === ' ') {
    wordCount++; // increment word counter
  }
}



If the last character is not a space, increment the wordCount counter.


const sentence = "The quick brown fox jumps over the lazy dog.";
for (let i = 0; i < sentence.length; i++) {
  const char = sentence.charAt(i);
  if (char === '.') {
    break; // exit loop when the point is reached
  }
  length++; // increment length counter
  if ('aeiou'.includes(char.toLowerCase())) {
    vowelCount++; // increment vowel counter
  }
  if (char === ' ') {
    wordCount++; // increment word counter
  }
}
if (sentence.charAt(sentence.length - 1) !== ' ') {
  wordCount++; // increment word counter if last character is not a space
}


Output the length of the sentence, the number of words in the sentence, and the number of vowels in the sentence.

console.log(`Length of sentence: ${length}`);
console.log(`Number of words: ${wordCount}`);
console.log(`Number of vowels: ${vowelCount}`);


Now When we run this code with the example sentence, the output should be:

Length of sentence: 44
Number of words: 9
Number of vowels: 11
