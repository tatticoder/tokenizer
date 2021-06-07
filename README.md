# tokenizer
Generate human readable pseudo random text strings

## To-do 
- Ask how many passwords [default 1] of how many sets [default 4] and seed [default time]
- Make go routines for concurrency and speed
- Use runes to change character set later
- Name of file to output to
- Go benchmark with sub tests 

## Calculating each character set
Generate a number [0,10) and based on that
- 0 - 6 → Alphabets
    - odd → uppercase
    - even → lowercase
- 7 - 8 → Digits
    - Print a number between 0000 to 9999
- 8 - 10 → characters
    - odd → pick 1 and repeat 4 times
    - even → pick 2 and repeat 2 times each

sample token generated : `TENT-1246-##@@-hand`