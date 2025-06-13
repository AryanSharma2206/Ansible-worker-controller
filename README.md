# 🛰️ Ansible Apache Automation on AWS EC2

This project demonstrates how to automate the installation of **Apache HTTP Server** on **two AWS EC2 worker nodes** using **Ansible** from a control node.

🔧 The Ansible control node sends commands via SSH to both worker nodes and installs Apache web server in a fully automated and repeatable manner.

---

## 📌 Project Architecture

Control Node (EC2)
|
| SSH (Port 22)
|
+------------+ +------------+
| Worker EC2 | | Worker EC2 |
| Node 1 | | Node 2 |
+------------+ +------------+
| |
|-- Apache Installed --|

yaml
Copy
Edit

---

## ⚙️ Tools & Technologies Used

- **Ansible** (Automation Tool)
- **AWS EC2** Instances
- **Ubuntu 22.04** (on all instances)
- **Apache2 Web Server**
- **SSH Key-based Authentication**

---

## 📂 Project Structure

```bash
ansible-control/
├── inventory
├── apache_install.yaml
├── ansible.cfg
├── screenshots/
│   ├── 1.PNG
│   ├── 2.PNG
│   ├── 3.PNG
│   ├── 4.PNG
│   ├── 5.PNG
│   ├── 7.PNG
🚀 Steps Performed
✅ Launched 3 EC2 Instances (1 Control + 2 Worker Nodes)

✅ Configured SSH Key-based login from control to workers

✅ Installed Ansible on Control Node

✅ Created inventory file listing both worker IPs

✅ Wrote a simple playbook to install Apache2

✅ Executed the playbook using:

bash
Copy
Edit
ansible-playbook -i inventory apache_install.yaml
🖼️ Screenshots
🔧 Setting Up Inventory File

🧪 Testing Ansible Connection

📜 Apache Playbook

🚀 Running the Playbook

✅ Apache Installed on Workers

🌐 Apache Homepage on Worker Nodes

📣 Conclusion
This project shows how powerful and simple Ansible can be for automating infrastructure tasks like web server installation across multiple nodes. It's scalable, secure, and ideal for repetitive server setup tasks.
---

**Aryan Sharma**  
B.Tech CSE (AI & DS) | Poornima University  
GitHub: [@AryanSharma2206](https://github.com/AryanSharma2206)  
LinkedIn: [linkedin.com/in/aryan-sharma2206](https://www.linkedin.com/in/aryan-sharma-a2a240353/)  
Location: Jaipur, India
---

