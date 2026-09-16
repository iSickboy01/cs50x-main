# Week 0 — Scratch

This was my first week of CS50. We started with the fundamentals of how computers represent information and then moved into algorithms, problem-solving, loops, and conditionals using Scratch.

## Binary and Bits
I learned about the binary system, which is the fundamental number system used by computers. Computers ultimately represent information using 0s and 1s.
I learned about bits and how different combinations of bits can represent different values.
A bit can have two possible values: 0 or 1.

Therefore:
1 bit = 2 possible values
2 bits = 4 possible values
8 bits = 2⁸ = 256 possible values
32 bits = 2³² possible values

I also learned about base conversion, particularly how numbers can be represented in different number systems.

## Bytes
I learned that:
1 byte = 8 bits

This is important because computers don’t just store numbers. They also use combinations of bits and bytes to represent things like characters, colours, images, sounds, and eventually entire programs.

## Representing Letters with Binary
I learned that computers can represent letters using numbers.
For example, under ASCII:
A = 65
B = 66
C = 67
…
a = 97
b = 98
…
These numbers can then be represented in binary.

For example:
A → 65 → 01000001

This means that the computer doesn’t inherently understand the letter “A”. It stores a numerical representation which software interprets as the letter A.

## ASCII
I learned about ASCII (American Standard Code for Information Interchange).
The original ASCII system used 7 bits, giving it 128 possible characters. Extended versions of ASCII used 8 bits and could represent 256 values, but standard ASCII itself was limited to 128 characters.
This limitation meant that ASCII wasn’t sufficient for representing all of the world’s languages and symbols.

## Text as Bytes
I learned that characters can be represented using bytes.
For example:
H + I + !
can be represented as three characters, with each character taking one byte in ASCII.

Therefore:
3 characters × 8 bits = 24 bits = 3 bytes
This helped me understand that even something as simple as a word is ultimately represented as binary information inside a computer.

## Uppercase and Lowercase Letters
I learned something interesting about ASCII: lowercase letters are 32 values higher than their uppercase equivalents.
For example:
A = 65
a = 97
And:
97 - 65 = 32
This means that there is a difference of one bit in their binary representations.
For example:
A → 01000001
a → 01100001
So changing the appropriate bit(particularly at the 2exp5 position 0r where the binary value is 32) can change an uppercase letter into its lowercase equivalent.

## Unicode
I learned about Unicode, which was developed to solve many of the limitations of ASCII.
Unicode can represent a huge range of characters from different writing systems, as well as symbols and emojis.
Unlike ASCII, Unicode is not limited to 256 characters. 

This allows computers to represent characters from many different languages, including characters that ASCII could never represent.

## Representing Colours
I learned that computers can represent colours using the RGB colour model:
R = Red
G = Green
B = Blue
Each RGB component can have a value from 0 to 255.
Since:
0–255 = 256 possible values = 2⁸, each colour channel requires 8 bits (1 byte).
Therefore, a typical RGB colour uses: 8 bits + 8 bits + 8 bits = 24 bits = 3 bytes
For example, a colour could be represented as:
RGB(255, 0, 0) - which represents pure red.

## Pixels and Images
I learned that when we zoom into a digital image, we eventually see tiny individual squares called pixels.
Each pixel contains information about its colour.
In a typical RGB image, each pixel can use 3 bytes (24 bits) to represent its colour.
Therefore, a large photograph can contain millions of pixels, with each pixel containing its own colour information.
This helped me understand that an image is ultimately just a huge collection of numerical data.

## Representing Sound
I also learned that computers can represent sound digitally.
Sound can be represented by measuring properties of a sound wave, such as:
Frequency
Amplitude
Duration
These measurements can be sampled and converted into numerical data, which can then be stored in binary.
This helped me see that computers can represent many seemingly different things—text, images, sound, etc.—using the same fundamental building blocks of bits and bytes.

## Programs and Interpretation
One of the important things I learned is that the computer ultimately works with zeros and ones, but software determines how those zeros and ones should be interpreted.
The same fundamental idea of binary representation can therefore be used to represent completely different kinds of information.

## Algorithms
I also learned about algorithms.
An algorithm is essentially a set of instructions or steps for solving a problem.
We looked at how algorithms can be designed to solve problems and how different algorithms can have different levels of efficiency.

## Return Values and Side Effects
I learned the difference between return values and side effects.
A return value is information that a function gives back to the program, while a side effect is an observable change or effect caused by the program, such as printing something to the screen.

## Loops and Conditionals
I also learned about:
Conditionals — allowing a program to make decisions.
Loops — allowing a program to repeat instructions.
These concepts became particularly important when we started using Scratch to build programs.
 