# Where are the Robots

## Description:
  Can you find the robots? https://jupiter.challenges.picoctf.org/problem/56830/ (link) or http://jupiter.challenges.picoctf.org:56830
  
## Solution
1. I open the instance. It gives a simple login page
   ![image](https://github.com/user-attachments/assets/b313b23a-1a62-4087-b1bc-28c421eb19d7)
2. So I go to the robots.txt of the page, which says to disallow one page.
   ![image](https://github.com/user-attachments/assets/0a1fb3d3-8dd7-42da-b34e-dfe042ed8f31)
3. This leads me to a .html page disallowed by the file.
   ![image](https://github.com/user-attachments/assets/caf3e3d5-00cd-4837-8e67-db100c721ecd)
4. So I go to the html disallowed by the site, giving me the flag ```picoCTF{ca1cu1at1ng_Mach1n3s_1bb4c}```
   ![image](https://github.com/user-attachments/assets/ec2d0cc8-47a3-4363-aa68-a78c453f1639)
