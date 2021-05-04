# Assessment 2

At HIGGZCODE we have a secret language. Lets say I want to say hi to someone secretly. I need to send them an "Encoded message". Here is how the encoding works. Lets start with a word.

Hello

For each letter, we need three numbers to represent that letter. The first two numbers are its placement index in the alphabet. in this example:

```
H => 08
e => 05
l => 12
l => 12
o => 15
```

the third letter will either be a 0 or a 1. It represents whether or not the letter is uppercase. For example.
The code for each letter would be

```
H => 081
e => 050
l => 120
l => 120
o => 150
```

a function that will take a sentence and will turn it into a string of digits. Please note the following exceptions.

a space (" ") character can be represented by the number 999.
a period (".") character can be represented by the number 666.

| input  |             Output |
| :----: | -----------------: |
|   a    |                010 |
|   A    |                011 |
|   z    |                260 |
|  Zaza  |       261010260010 |
| A dog. | 011999040150070666 |

To test your function, please send me what the following sentence outputs from your function.

The quick brown fox jumped over the fence. I love sauerkreut."
