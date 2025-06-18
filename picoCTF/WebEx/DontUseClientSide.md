# dont-use-client-side

## Description
Can you break into this super secure portal? https://jupiter.challenges.picoctf.org/problem/29835/ (link) or http://jupiter.challenges.picoctf.org:29835

## Solution
1. The site is just a normal login page. I try a random password, but it gives me ```incorrect password```.
   ![image](https://github.com/user-attachments/assets/934f4242-896c-4c29-a3be-5c78473fa439)
   ![image](https://github.com/user-attachments/assets/e55361bd-5623-4433-9052-87e0966b7942)
2. So now I inspect the page, where I see a code for a script.
   ![image](https://github.com/user-attachments/assets/ecf182de-33ba-4200-bc45-c1dd80fd5901)
3. Upon opening the script, I notice that the flag is spliced into various parts, and I have to join them together.
   ![image](https://github.com/user-attachments/assets/2157fe49-b938-4f13-a44a-01f127dd57af)
4. Upon concatenating all the substring together, I get ```picoCTF{no_clients_plz_7723ce}```
5. Now I try this password and I get ```password verified```. The flag is also the same.
   ![image](https://github.com/user-attachments/assets/a2b0cbe1-58b4-4c7c-86e2-59e3b4736b0e)
