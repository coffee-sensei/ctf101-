# Bit-O-Asm 1

## Question Statement
Can you figure out what is in the ```eax``` register? Put your answer in the picoCTF flag format: ```picoCTF{n}``` where n is the contents of the eax register in the decimal number base. If the answer was ```0x11``` your flag would be ```picoCTF{17}```.
Download the assembly dump here.

## Solution
1. I download the assembly dump.
   ![image](https://github.com/user-attachments/assets/f99e4eaf-7c84-4aff-976f-25ef38e076d9)
2. In line 6, beside ```eax```, the ASCII number ```0x30``` is written.
3. Upon converting to decimal from ASCII, I get 48.
4. The flag is ```picoCTF{48}```.
