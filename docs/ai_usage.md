AI Use Log
Tool/Model Used: Gemini 1.0 Pro

Task P4.1 – Data Types:
I asked Gemini to provide examples of the three fundamental Python data types: strings, integers, and floats. I also requested an explanation of how the type() function can be used to check a variable’s data type.
At first, I only wrote the code, but later I improved it by adding print() statements along with the actual outputs. This way, the examples clearly demonstrated what type() returns for each case. I also formatted the response in Markdown so it would be cleaner and easier to read.
To confirm accuracy, I ran the code locally with test values (x = "Hello, world!", y = 10, z = 3.14) and verified that the outputs matched the expected results (str, int, and float).

Rosalind Problems

Problem 1 (P6.2):
The task required calculating the square of a right triangle’s hypotenuse. I used the input() function to collect the side lengths from the user and then converted them to floats. The formula a**2 + b**2 was correctly applied to compute the result.

Problem 2 (P8.3):
This exercise focused on string and list slicing. I wrote code that read a string and four integers, then extracted two substrings using Python slicing. Since Python’s slice operation excludes the end index, I added +1 to ensure the last character was included (s[a:b+1], s[c:d+1]).

Problem 3 (P12.3):
Here, I needed to sum all odd numbers within a given range. Using range(a, b+1) to generate the sequence and if n % 2 == 1 to filter odd numbers, I implemented a concise solution with a generator expression inside sum().

Problem 4 (P15.2):
This problem dealt with file handling. By reading a text file line by line in a for loop and using enumerate to track line numbers, I was able to print only the even-numbered lines from practice.txt.

Problem 5 (P18.2):
The goal was to perform a word count. I split the file content into words with split() and then used collections.Counter to tally occurrences efficiently. Finally, I iterated over the dictionary to print each word and its frequency.

Problem 6 (P19.1):
This problem asked for counting nucleotides (A, C, G, T) in a DNA sequence. I solved it using the string method .count(), which allowed me to directly count occurrences of each base.

Problem 7 (P21.1):
I had to transcribe DNA into RNA. Using Biopython’s Seq object, I applied the .transcribe() method, which replaced all thymine (T) bases with uracil (U) to form the RNA sequence.

Problem 8 (P21.2):
The task was to translate RNA into a protein sequence. Again using Biopython’s Seq, I applied .translate(to_stop=True). This translated the RNA codons into amino acids and stopped automatically at the first stop codon.

Problem 9 (P23.2):
The challenge was to find the FASTA record with the highest GC content. By iterating through sequences using Bio.SeqIO.parse and applying gc_fraction() from Bio.SeqUtils, I calculated GC content for each record and tracked the sequence with the highest percentage along with its ID.
