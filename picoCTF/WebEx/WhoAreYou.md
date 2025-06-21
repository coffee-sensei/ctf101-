![image](https://github.com/user-attachments/assets/e797825a-3649-4572-a0a9-9fc3f0d2e412)# Who Are You

##

## Solution
1. I open the website on my browser, but it does not allow me to access it.
![image](https://github.com/user-attachments/assets/ff11e5b8-d928-4e85-a345-d55fbc3ebbb4)
2. SO I open it on Burp. Since it says ```Only people who use the official PicoBrowser are allowed on this site!```, I change the User agent to PicoBrowser.
   ![Screenshot from 2025-04-16 19-06-19](https://github.com/user-attachments/assets/baad25ba-800f-4d6b-b678-66f7a15a245f)
3. Now the website says I don't trust users from other sites.
   ![image](https://github.com/user-attachments/assets/ccd6d015-6544-4b17-ae8d-1ad7bf009ef3)
4. So I add a referer which tells from which site I am accessing the website.
   ![image](https://github.com/user-attachments/assets/4f79babb-291a-468d-b7a1-473cc05c6a91)
5. However, we still havent solved it as the site now updates to whatever is shown below
   ![image](https://github.com/user-attachments/assets/c0666fa6-e119-4d49-8832-4ecd7a15a279)
6. So now we add DNT which means Do Not Track as 1, as websites understand that they should not track websites.
   Once we do this and send this to the server, we get the website showing this:
   ![image](https://github.com/user-attachments/assets/cd6a664f-3e97-4beb-8ea4-d6e38038c482)
7. So we take the website back in time, and add a line in the proxy:
   ``` bash
   Date: 29 Nov 2018
   ```
   Now we reload, and the site gives us one more problem.
   ![image](https://github.com/user-attachments/assets/424a1222-1e26-4945-8a56-b6efa69b22db)
8. For this we find a Swedish IP address along with the code: ```X-Forwarded-For: 192.44.242.1```
   Now we reload, when it gives me this:
   ![image](https://github.com/user-attachments/assets/d8b32661-4f8f-4cd3-a7df-8fbf47dc41b6)
9. So we now add a language code ```Accept-Language: sv-SE,sv;q=0.9```
10. This gives me the flag: ```picoCTF{http_h34d3rs_v3ry_c0Ol_much_w0w_8d5d8d77}```
![image](https://github.com/user-attachments/assets/0fb76a0a-5127-4fa0-9fef-67adf86a4466)

   
