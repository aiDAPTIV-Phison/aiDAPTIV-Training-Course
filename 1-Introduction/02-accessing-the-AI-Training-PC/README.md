# Accessing the AI Training PCs

In this lesson, you’ll learn how to set up VPN access and remotely connect to a **Phison AI Training PC (AITPC)**.  
You’ll need to complete these steps before you can run the hands-on labs in this course.  

<p align="center">
  <a href="https://youtu.be/Y3x4cn6vZvQ">
    <img src="https://github.com/aiDAPTIV-Phison/aiDAPTIV-Training-Course/blob/e60ff9d6c3597c4d2f8de5ea3f2bef1f96b82fdd/assets/Remote_Access_Guide.png" width="600" alt="Remote Access Guide">
  </a>  
  <br>
  ▶️ <em>Click the image above to watch the video on YouTube.</em>
</p>

---

## Step 1: Install the VPN Client (CATO)

We use **CATO Networks VPN** for secure access.  

1. Download the client here:  
   👉 [CATO Client Download](https://clientdownload.catonetworks.com/)  

2. Install the client and open the **CATO app**.  

---

## Step 2: Log Into the VPN

1. Open the **CATO app**.  
2. Enter the username and password provided to you by the admin.  
3. Wait 5–10 seconds for the connection to verify.  
4. Once connected, you’ll be securely on the Phison VPN.  

---

## Step 3: Configure Host File 

### Windows
For Windows users, you’ll need to update the host file to map the jump server address.  

1. Open the host file with admin privileges: C:\Windows\System32\drivers\etc\hosts
2. Add this line at the bottom: 10.102.10.20 phisongenai.phison.com
3. Save and close the file.  

### macOS / Linux
For macOS and Linux users, the process is very similar.  

1. Open **Terminal** (use Spotlight Search with `Command + Space` and type “Terminal”). 
2. Edit the hosts file with root privileges: 
```bash
sudo nano /etc/hosts
```
You’ll be prompted for your computer password.
3. Add this line at the bottom: 10.102.10.20 phisongenai.phison.com
4. Save and exit (Ctrl+O, Enter, Ctrl+X in nano).

---

## Step 4: Remote into the AI Training PC

Once connected to the VPN, you can log into the **jump server**:  

👉 [phisongenai.phison.com](https://phisongenai.phison.com)  
(*Note: This link only works when you are connected to the VPN.*)  

---

## ✅ You’re Ready

You now have secure access to the Phison **AI Training PCs (AITPCs)**.  
From here, you’ll be able to run datasets, fine-tuning jobs, and inference for the aiDAPTIV+ training course.
