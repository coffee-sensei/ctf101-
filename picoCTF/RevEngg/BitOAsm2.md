# Bit-O-Asm 2

## Question statement
Can you figure out what is in the eax register? Put your answer in the picoCTF flag format: picoCTF{n} where n is the contents of the eax register in the decimal number base. If the answer was 0x11 your flag would be picoCTF{17}.
Download the assembly dump here.

## Solution
1. Downloaded file
  ![image](https://github.com/user-attachments/assets/ca5e40f2-1a39-4ccc-a73b-fe487ff6171c)
2. Found at eaf value was pointing towards ```DWORD PTR [rbp-0x4]```, which had the value ```0x9fe1a```.
3. Upon converting, we get 654874.
4. The flag is picoCTF{654874}.
