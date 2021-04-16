In NetBeans, open the project called ‘Task1’ and inspect the data file provided called datafile.txt. This file
contains a passage of text that is encoded. You are not required to, and should not, alter this text file i.e., it is
intended to be read-only.
The encoded data file uses a very simple cipher based on the encryption of the positions of vowels and
consonants from the English alphabet. These positions (with respect to the cipher that is employed) are
illustrated in Tables 1 and 2. Note that for the purposes of this cipher the letter y (or Y) is counted as a vowel.

1 a 2 A 3 e 4 E 5 i 6 I 7 o 8 O 9 u 10 U 11 y 12 Y

Table 1: vowel positions

1 b 2 B 3 c 4 C 5 d 6 D 7 f 8 F 9 g 10 G
11 h 12 H 13 j 14 J 15 k 16 K 17 l 18 L 19 m 20 M
21 n 22 N 23 p 24 P 25 q 26 Q 27 r 28 R 29 s 30 S
31 t 32 T 33 v 34 V 35 w 36 W 37 x 38 X 39 z 40 Z

Table 2: consonant positions

The cipher works by substituting the relevant alphabet character for the position based on the tables. During
the encoding of a passage of text, a vowel is denoted by inserting the letter ‘V’ followed directly by its
position index. For example, the uppercase letter ‘A’ is encoded as ‘V2’. Similarly, a consonant is encoded by
inserting the letter ‘C’ followed directly by its position index. For example, the lowercase letter ‘h’ is encoded
as ‘C11’. For example, the word Apples would be encoded as V2C23C23C17V3C29.
To keep this deciphering task even simpler, the encoded data file has no punctuation and comprises only
words separated by whitespace (and newlines).

Your task is to write a Java 8 program (as a NetBeans 8 project) that opens the data file, parses the
characters in the data file, deciphers them to normal text and prints the decoded passage of text to the
console. Newlines and blank lines must be maintained in the decoding.
In addition to the console output, your program should also save all the output to a text file in the NetBeans
project root folder. Name the file results.txt.
Having performed these actions, your program should close the opened.
