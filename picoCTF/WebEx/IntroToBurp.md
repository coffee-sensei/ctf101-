# IntroToBurp


## Solution
1. The instance is a basic registration form.
  ![image](https://github.com/user-attachments/assets/637f7893-0827-428f-99fb-92fc05536059)
2. In the 2-factor authentication, it fails, giving ```Invalid otp```
   ![image](https://github.com/user-attachments/assets/b08cfa03-aa53-4225-9180-28a294661f38) ![image](https://github.com/user-attachments/assets/a03f1622-1dfc-4bf2-a8cd-0f990cadd5e2)
3. To tackle this, we open the instance in PortSwigger, a browser of Burp Suite.
4. Once we reach the top, we type in the otp and click on submit. Here, Burp will be holding back or intercepting the data to be sent to the server until we authorise it. We now send it forward and check.
   ![image](https://github.com/user-attachments/assets/aa0987a1-22da-4178-a710-6708d9f5bac1) ![image](https://github.com/user-attachments/assets/40a2c8c5-f205-4494-8df2-4e71955ba59c)
5. We see that a new value, otp, is being sent. We remove this line and forward it to the server.
   ![image](https://github.com/user-attachments/assets/7968fe6c-ba60-4df3-b364-b59de800d192)
6. This gives us the flag.
   ![image](https://github.com/user-attachments/assets/4f195d19-7a55-4e95-8afc-c74decf92cc2)
```picoCTF{#0TP_Bypvss_SuCc3$S_6bffad21}```
