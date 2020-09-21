# BBCodeChallenge
Coding Challenge Problems for Best Buy Application

Why I used this sequence:
  Since worst case for prime is N(when it is prime) and best case is just one division, I figured this would be the big bottleneck in the program. Doing some research I saw that there are 664,579 prime numbers below 10,000,000(https://primes.utm.edu/howmany.html). I figured instead of checking if every number is prime and palindromic, I would instead generate a set of all the 10^4 7 digit palindromes, create a set of all primes within this set, then iterate through pi and see if our 7 digit string was a member of the set. 
 
Process:
  There are 10^4 7 digit palindromes and after finding out which ones are prime it widdled down possible solutions to 668. I added each possible 7 digit prime palindrome to a set for quick lookup. The next step was to simply iterate through a splice of the string of pi. First I had to remove the period, but after that this was a simple lookup in our constructed set of possibilities. I found the solution on the 13,901 th iteration with a solution of 9149419.
