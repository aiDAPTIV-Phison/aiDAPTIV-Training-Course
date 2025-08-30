# Accessing the AI Training PCs

In this lesson, you’ll learn how to set up VPN access and remotely connect to a **Phison AI Training PC (AITPC)**.  
You’ll need to complete these steps before you can run the hands-on labs in this course.  

<p align="center">
  <a href="https://youtu.be/_Kw96F9KpUA">
    <img src="https://github.com/aiDAPTIV-Phison/aiDAPTIV-Training-Course/blob/b56a14310073724f67f66e5bcb0f4cc7b24752ed/assets/Remote_Access_Guide.png" width="600" alt="Remote Access Guide">
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

## Step 3: Configure Host File (Windows Only)

For Windows users, you’ll need to update the host file to map the jump server address.  

1. Open the host file with admin privileges: C:\Windows\System32\drivers\etc\hosts
2. Add this line at the bottom: 10.102.10.20 phisongenai.phison.com
3. Save and close the file.  

*(Mac/Linux users do not need to update this step.)*  

---

## Step 4: Remote into the AI Training PC

Once connected to the VPN, you can log into the **jump server**:  

👉 [phisongenai.phison.com](https://phisongenai.phison.com)  
(*Note: This link only works when you are connected to the VPN.*)  

---

## ✅ You’re Ready

You now have secure access to the Phison **AI Training PCs (AITPCs)**.  
From here, you’ll be able to run datasets, fine-tuning jobs, and inference for the aiDAPTIV+ training course.
