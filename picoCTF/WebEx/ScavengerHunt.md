# Scavenger Hunt

## Description
There is some interesting information hidden around this site http://mercury.picoctf.net:39491/. Can you find it?

## Solution
![image](https://github.com/user-attachments/assets/e424c940-e7bc-49a2-b177-20ee671d13fd)
1. This is the site, with just 2 clickable buttons, how and what
2. I open the inspect tool, where i get the first part of the flag.
   ![Screenshot from 2025-06-11 19-15-52](https://github.com/user-attachments/assets/04b8aac2-882f-4fcb-aa96-001c0435fdbf)
3. Upon further looking in ```mycss.cs```, I get the second part of the flag.
   ![Screenshot from 2025-06-11 19-16-18](https://github.com/user-attachments/assets/ad6c542a-6f05-4ae2-ad6b-a8d30eb8cceb)
4. Now I check ```myjs.js``` where I see the question - What can I do to stop Google from indexing my website? This implies that the website has a robots.txt page to stop indexing of the site.
