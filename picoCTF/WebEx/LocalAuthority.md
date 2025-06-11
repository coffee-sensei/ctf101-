# Local Authority

## Description
Can you get the flag?
Additional details will be available after launching your challenge instance.

## Solution
1. The question launches the website ```http://saturn.picoctf.net:52912/```. It is a site with a login page as shown below
   ![image](https://github.com/user-attachments/assets/84fadfc5-5f9f-482d-aad6-a3d6411fed38)
2. I first try admin as username and password, which gives me this:
   ![image](https://github.com/user-attachments/assets/dcb90811-35a6-433d-953f-d0d207320a32)
3. Since this didnt work, I inspect the site, and enter a wrong password and username again.
4. In the Inspect of ```login failed``` page, I see a ```secure.js``` script, which reveals the password and username which gives the right login credentials.
   ![image](https://github.com/user-attachments/assets/4412ea1c-af26-49a5-832b-5e76d609049a)
5. I use this password and username which logs me in and gives me the flag.
   ![image](https://github.com/user-attachments/assets/bf1d48b9-9383-40f8-8b10-410f25e257cc)
6. The flag is ```picoCTF{j5_15_7r4n5p4r3n7_a8788e61}```.
