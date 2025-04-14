## 🛡️ Offensive Security Intro

**Room:** [Offensive Security Intro — TryHackMe](https://tryhackme.com/room/offensivesecurityintro)  
**Status:** ✅ Completed  
**Date:** *(29 March 2025)*  
**Category:** Pre-Security → Introduction to Cyber Security  

---

### 📌 Objective

Hack a simulated website in a safe, legal environment to get a hands-on feel for what an ethical hacker does. This room is a beginner-friendly entry point into offensive security.

---

### 🛠️ Tools Used

- **Virtual Machine (VM)** – Provided by TryHackMe to simulate a real environment for hacking.
- **Linux Terminal** – Used on the VM to run commands and interact with tools.
- **Gobuster** – A command-line tool used to brute-force web directories and find hidden pages.

---

### 🧪 Steps Taken

1. Launched the provided virtual machine (VM) with a simulated banking website called **FakeBank**.
2. Opened the **Linux terminal** in the VM for command-line access.
3. Ran the following Gobuster command to enumerate hidden directories:

gobuster -u http://fakebank.thm -w wordlist.txt dir


- `-u` specifies the URL.
- `-w` uses a wordlist of potential directories.

4. Found a hidden page: `/bank-transfer`.
5. Accessed this page to simulate a transfer of money between accounts, replicating a typical vulnerability exploit.

---

### 🧠 What I Learned

- How to **think like a hacker**, spotting what might be missed by developers or admins.
- How ethical hackers use tools like **Gobuster** to uncover hidden areas of a website.
- The basics of **web application penetration testing**.
- The **importance of securing hidden pages**, which can be a major risk if exposed.

---

### 🚧 Challenges Faced

- First time using **Linux**, so navigating the terminal and understanding commands was new territory.
- Needed to get used to reading terminal output and interpreting what each result meant.

---

### 💭 Reflections

This was a really enjoyable first experience in hands-on hacking. It gave me a taste of the mindset needed to work in **Offensive Security** — where you're not just clicking around, you're thinking like an attacker. It also reinforced the importance of strong security practices for websites.

The fact that a simple tool like Gobuster could uncover sensitive pages was eye-opening. I can see how, with permission, a penetration tester could help companies spot these weaknesses before real attackers do.
