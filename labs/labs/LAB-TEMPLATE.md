# LAB: <Offensive Security Intro> — TryHackMe (Sanitized notes)

Room: <Offensvive Security Intro>
Date completed: 2025-03-26
Difficulty: Beginner 

Overview:
- In this Room, we talk about Offensie Security, and it envolves breaking into computer systems, exploiting software bugs, and finding loopholes in applications to gain unauthorized access. The goal is to understand hacker tactics and enhance our system defencesthe Goal is to show you how an ethical hackers operates.
The problem: Most companies have an admin portal page, giving their staff access to basic admin controls for day-to-day operations. For a bank, an employee might need to transfer money to and from client accounts. Due to human error or negligence, there may be instances when these pages are not made private, allowing attackers to find hidden pages that show or give access to admin controls or sensitive data.

Tools used:
- gobuster

What I did (safe version):
1. To begin i typed this command into the terminal gobuster: -u http://fakebank.thm -w wordlist.txt dir.
2. This command helped me find potentially hidden pages on FakeBank's website using Gobuster.
3. Gobusters will scan the website with each word in the list, finding pages that exist on the site.
4. Gobuster will have told you the pages in the list of page/directory names (indicated by Status: 200).
5. I found a secret bank transfer page that allows you to transfer money between bank accounts (/bank-transfer).
6. I typed the hidden page into the FakeBank website using the browser's address bar.

Commands I used (-u , -w): -u is used to state the websites we are scanning, and -w takes a list of of words to iterate through to find hidden pages.
