# Word Count
## A Word Counting Application for Epicodus C# BDD Code Review _10.20.2017_

### By Kimberly Bordon

## Description
_This is an application that exercises Behavior-Driven Development C# in taking a word from a user, and counting its occurrences from a user-provided block of text._

## Specifications

| Behavior | Input Example| Output Example|
|-|-|-|
| When the user enters a word to count, it will store that word and show it on the next page. | cat | You entered: cat |
| If the user enters non-alphabetical letters or numbers in their word, it will still store that word. | Kat3 | You entered: Kat3 |
| When the user enters a word to count, and their desired block of text to count from, it will store both and show them on the next page. | cat <br><br>I love my cat Grindel, she's the coolest cat that ever did cat. | You entered: cat<br><br>Text:<br>I love my cat Grindel, she's the coolest cat that ever did cat. |
| When the user enters a single letter word to count, and the same word to count from, it will count it once. | a <br> a | You entered: a <br> Counted: 1 <br><br>Text:<br> a |
| When the user enters a single letter word to count, and a different single letter word to count from, it will count zero. | a<br> i | You entered: a <br> Counted: 0<br><br> Text:<br> i |
| When the user enters a single letter word, and the same word but in different casing, it will not consider it an exact match, and will still count it zero. | a<br> A | You entered: a <br> Counted: 0<br><br>Text:<br> A |
| When the user enters a single letter word, and a group of the same word to count from, it will count it however many times it appears. | a<br> a a a a a | You entered: a<br> Counted: 5<br><br> Text:<br>a a a a a|
| When the user enters a single letter word, and a group of a different single letter word, it will count it zero. | a<br> i i i i i | You entered: a<br>Counted: 0<br><br>Text:<br>i i i i i<br>|
| When the user enters a single letter word, and a group of the same word but in different casing, it will not consider them to an exact match, and it will still count them zero times. | a<br> A A A A A | You entered: a<br>Counted: 0<br><br>Text:<br> A A A A A|
| When the user enters a single letter word, and a group of different single letter words, it will only count the exact matches. | a<br> A a a i A | You entered: a<br>Counted: 2<br><br> Text:<br>A a a i A|
| When the user enters a single letter word, and a multiple letter word, it will count zero. | a<br> at | You entered: a<br>Counted: 0<br><br>Text:<br>at |
| When the user enters a single letter word, and a single letter word that has a punctuation mark, it will ignore punctuation and count the word. | I<br>I, | You entered: I<br>Counted: 1<br><br>Text:<br>I,
| When the user enters a multiple letter word, and the same word, it will count the word once. | dog<br>dog<br> | You entered: dog<br>Counted: 1<br><br>Text:<br>dog|
| When the user enters a multiple letter word, and a different word, it will count zero. | dog<br> Lassie | You entered: dog<br>Counted: 0<br><br>Text:<br>Lassie|
| When the user enters a multiple letter word, and the same word, it will only count the word if it is an exact match with the same casing, and no partial matching. | dog<br>Dog | You entered: dog<br>Counted: 0<br><br>Text:<br>Dog|
| When the user enters a multiple letter word, and the same word but with a punctuation mark, it will ignore the punctuation mark and still count the word. | dog<br>dog! |You entered: dog<br>Counted: 1<br><br>Text:<br>dog!|
| When the user enters a word, and a group of the same word, it will count that word however many times it appears. | dance<br>dance dance dance | You entered: dance<br>Counted: 3<br><br>Text:<br>dance dance dance|
| When the user enters a word, and a group of different words, it will count that word zero times. | dance<br> I am a wallflower | You entered: dance<br>Counted: 0<br><br>Text:<br> I am a wallflower |
| When the user enters a word, and any desired block of text to count from, it will count only that exact match. | dance<br>Dance no I will not dance for dancer I am not| You entered: dance <br>Counted: 1<br><br>Text:<br>Dance no I will not dance for dancer I am not |
| When the user enters a word, and any desired block of text to count from, it will only count that exact match, ignoring punctuation marks. | dance<br>Dance? No, I will not dance, for dancer I am not!| You entered: dance <br>Counted: 1<br><br>Text:<br>Dance? No, I will not dance, for dancer I am not!  |
| If the user enters more than a single word to count in the form, it will count each word matched exactly to the block of text to count from, ignoring punctuation. | I dance<br>Dance? No, I will not dance, for dancer I am not! | You entered: I <br>Counted: 2<br><br> You entered: dance <br>Counted: 1<br><br>Text:<br>Dance? No, I will not dance, for dancer I am not! |

## Setup/Installation Requirements
**At this moment, this project only consists of a README.md, but in the future it will require the .NET framework for installation, and will provide those necessary instructions.**
* Enter the URL: https://github.com/kbordon/csharp-week2-code-review in your browser, and the project page will display the README.md below the table of file links.
* Or, if you'd prefer to view the README.md locally, using your terminal or powershell, clone this repository by typing ">git clone https://github.com/kbordon/csharp-week2-code-review.git"
    * Alternatively, you can use a browser to download the .zip file from the Github web interface at the URL: https://github.com/kbordon/csharp-week2-code-review
* Navigate to the project folder csharp-week2-code-review, and use a text editor like Atom to open the README.md.

## Support and contact details

_If you have any questions, comments, or concerns, please contact Kimberly at [kbordon@gmail.com](mailto:kbordon@gmail.com)._

## Technologies Used

* Atom
* GitHub
* _TBA_

### License

*This software is licensed under the MIT license.*

Copyright © 2017 **_Kimberly Bordon_**
