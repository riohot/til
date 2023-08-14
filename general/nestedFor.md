# Nested for Loops

- A program describes a sequence of operations for the PC to perform
- Among those operations may be some SUBSEQUENCES that the PC should repeat multiple times

- In some cases, a repeating subsequence of operations itself contains a SUBSEQUENCE of operations that
  should be repeated multiple times as part of performing the one iteration of the consttaining sequence.

Example: algorithm for cleaning the windows in my house

```bash
    1. Get cleaning supplies from the closet
    2. If there are no more dirty windows then stop, ELSE
    3. Go to the next dirty window
        1a. Spray cleaner
        1b. Wipe window
        1c. If its not clean enough go back to step 1a
    4. Go back to step 2
```

This has two loops

1. Outer one comprising every step except the 1st
2. Inner one comprising 1a-1c

- Both would likely have different COUNTS (i < n) that they have to work with

- Loop count
  You dont know how many times the program will need to run through a given loop.

Something has to change from iteration to iteration, else the loop will never end

QUESTION - is there any scenario in which we would want to BREAK out of the loop ourselves rather than run it nLOOP times?
