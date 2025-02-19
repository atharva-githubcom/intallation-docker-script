## 📖 How to Use

### **1️⃣ Running the Script on AWS EC2**
There are **two methods** to use this script:

### **Method 1: Add Script in EC2 User Data (Recommended)**
This method will **automatically install Docker** when launching an EC2 instance.

1. **Go to AWS EC2 Console**  
2. Click **Launch Instance**  
3. Choose **Ubuntu 22.04 or 20.04 AMI**  
4. Select an **Instance Type** (e.g., `t2.micro` for free tier)  
5. Scroll down to **Advanced Details**  
6. Find the **User Data** section  
7. Copy and paste the script (provided in this repository) into **User Data**  
8. Complete the configuration and **Launch the instance**  

🚀 **Docker will be installed automatically once the instance starts!**  

---

Running the Script on a Virtual Machine (VM)
If you're using a local VM (e.g., VirtualBox, VMware, KVM, or Proxmox) running Ubuntu, follow these steps:

Open the terminal in your VM
Download the script 
1. wget paste the link of my github
Make the script executable
2.chmod +x docker-install.sh
Run the script with sudo
3.sudo ./docker-install.sh
✅ Docker will be installed on your VM automatically!

🎯 How to Verify Docker Installation
After running the script, check Docker installation:
docker --version
