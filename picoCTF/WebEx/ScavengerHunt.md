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
   ![Screenshot from 2025-06-11 19-16-07](https://github.com/user-attachments/assets/47d5e86d-9543-44f2-a56b-5b220cdf8f37)
5. So I check the robots.txt as well, which gives me part 3 of the flag.
   ![Screenshot from 2025-06-11 19-15-29](https://github.com/user-attachments/assets/3709c47a-8bc7-461f-bd6d-343ebf314a2f)
6. It gives the hint that this is an Apache server, which means it has hidden files like ```/.htaccess```.
7. I try ```/.htaccess```, which gives me part 4 of the flag.
   ![Screenshot from 2025-06-11 19-17-37](https://github.com/user-attachments/assets/88db1b76-0c67-4952-8ef8-a772bc6ac58a)
8. Here it states that the dev makes sites on Mac and Mac has a file where it stores data called as ```/.DS_Store```, which I access. This gives me the final part of the flag.
   ![Screenshot from 2025-06-11 19-18-38](https://github.com/user-attachments/assets/67d5c4ae-4ef2-4d32-84d1-443a7c6c8004)
9. The flag is ```picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_f7ce8828}```.
