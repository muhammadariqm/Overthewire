# 🕶️ CYBER SECURITY WARGAMES LOG

```
██╗  ██╗ █████╗  ██████╗██╗  ██╗███████╗██████╗ 
██║  ██║██╔══██╗██╔════╝██║ ██╔╝██╔════╝██╔══██╗
███████║███████║██║     █████╔╝ █████╗  ██████╔╝
██╔══██║██╔══██║██║     ██╔═██╗ ██╔══╝  ██╔══██╗
██║  ██║██║  ██║╚██████╗██║  ██╗███████╗██║  ██║
╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝
```

> Cyber Security learning journey through OverTheWire Wargames

![Linux](https://img.shields.io/badge/Linux-Terminal-black?style=for-the-badge&logo=linux)
![CTF](https://img.shields.io/badge/CTF-Practice-red?style=for-the-badge)
![Cyber](https://img.shields.io/badge/CyberSecurity-Learning-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Progress-Ongoing-blue?style=for-the-badge)

---

# 🧠 About

Repository ini berisi dokumentasi perjalanan saya menyelesaikan challenge dari **OverTheWire Wargames**.

Skill yang dipelajari:

- Linux Command Line
- Networking
- Cryptography dasar
- Web Security
- Privilege Escalation
- Git
- CTF Problem Solving

---

# ⚔️ Wargame Progress

```
Bandit   ██████████████████████████░░░  33/34
Natas    ████████████████░░░░░░░░░░░░  14/34
```

---

# 🐧 Bandit Wargame

## Level 1
Password
```
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```

---

## Level 2
```
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
```

---

## Level 3
```
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```

---

## Level 4
```
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```

---

## Level 5
```
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```

---

## Level 6
```
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```

---

## Level 7
```
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```

---

## Level 8
```
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
```

---

## Level 9
```
4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
```

---

## Level 10
```
FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
```

---

## Level 11
```
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
```

---

## Level 12
```
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
```

---

## Level 13
```
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```

---

## Level 14

Command
```
echo "MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS" | nc 127.0.0.1 30000
```

Password
```
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
```

---

## Level 15

Command
```
echo "8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo" | openssl s_client -connect localhost:30001 -quiet
```

Password
```
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
```

---

## Level 16

Scan port

```
nmap -p 31000-32000 127.0.0.1
```

Open ports

```
31046
31518
31691
31790
31960
```

SSL test

```
echo "kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx" | openssl s_client -connect 127.0.0.1:31790 -quiet
```

Login

```
ssh -i key17 bandit17@bandit.labs.overthewire.org -p 2220
```

---

## Level 17

```
EReVavePLFHtFlFsjn3hyzMlvSuSAcRD
```

---

## Level 18

Correct password

```
x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
```

Diff output

```
42c42
< x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
---
> pGozC8kOHLkBMOaL0ICPvLV1IjQ5F1VA
```

---

## Level 19

```
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
```

Command

```
cat /etc/bandit_pass/bandit19
```

---

## Level 20

```
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
```

---

## Level 21

```
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
```

---

## Level 22

```
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
```

---

## Level 23

Cronjob analysis

```
cat /etc/cron.d/cronjob_bandit23
```

MD5 generate

```
echo I am user bandit23 | md5sum | cut -d ' ' -f 1
```

Output file

```
/tmp/8169b67bd894ddbb4412f91573b38db3
```

Exploit script

```
echo 'cat /etc/bandit_pass/bandit24 > /tmp/ambil24' > /tmp/script.sh
```

Password

```
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
```

---

## Level 25

```
iCi86ttT4KSNe1armKiwbQNmB3YJP3q4
```

SSH key login

```
ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220
```

---

## Level 27

```
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB
```

Git clone

```
git clone ssh://bandit28-git@bandit.labs.overthewire.org/home/bandit28-git/repo
```

---

## Level 28

```
Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN
```

---

## Level 29

```
4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7
```

---

## Level 30

```
qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL
```

---

## Level 31

```
fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy
```

---

## Level 32

```
3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K
```

---

## Level 33

```
tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0
```

---

# 🌐 Natas Wargame

## Level 4
```
QryZXc2e0zahULdHrtHxzyYkj59kUxLQ
```

---

## Level 5
```
0n35PkggAPm2zbEpOU802c0x0Msn1ToK
```

---

## Level 6
```
0RoJwHdSKWFTYR5WuiAewauSuNaBXned
```

---

## Level 7
```
bmg8SvU1LizuWjx3y7xkNERkHxGre0GS
```

---

## Level 8
```
xcoXLmzMkoIP9D7hlgPlh9XD7OgLAe5Q
```

---

## Level 9
```
ZE1ck82lmdGIoErlhQgWND6j2Wzz6b6t
```

---

## Level 10
```
t7I5VHvpa14sJTUGV0cbEsbYfFP2dmOu
```

---

## Level 11
```
UJdqkK1pTu6VLt9UHWAgRZz6sVUZ3lEk
```

---

## Level 12
```
yZdkjAYZRd3R7tq7T5kXMjMJlOIkzDeB
```

---

## Level 13
```
trbs5pCjCrkuSknBBKHhaBxq6Wm1j3LC
```

---

## Level 14
```
z3UYcr4v4uBpeX8f7EZbMHlzK4UR2XtQ
```

SQL Injection

```
sqlmap -u "http://natas14.natas.labs.overthewire.org/" --data "firstname=sql&submit=Submit" --dbs --random-agent

sqlmap -u "http://natas14.natas.labs.overthewire.org/" --data "number=3&submit=Submit" --dbs --random-agent
```

---

## Level 15
```
SdqIqBsFcz3yotlNYErZSZwblkm0lrvx
```

## Level 16
```
hPkjKYviLQctEW33QmuXL6eDVfMW4sGo
```

## Level 17
```
EqjHJbo7LFNb8vwhHb9s75hokh5TF0OC
```

## Level 18
```
6OG1PbKdVjyBlpxgD4DDbRG6ZLlCGgCJ
```

## Level 19
```
p5mCvP7GS2K6Bmt3gqhM2Fc1A5T8MVyw
```

# 🛠 Tools Used

- Linux Terminal
- Nmap
- Netcat
- OpenSSL
- Git
- sqlmap
- Brupsuite
  
---

# 📚 References

https://overthewire.org/wargames/

---

# 👨‍💻 Author

```
Name : Muhammad Ariq
Role : Cyber Security Learner
Focus: Web Security | Linux | CTF
```

GitHub

```
https://github.com/muhammadariqm
```

---

# ☠️ Motto

```
Learning to break systems in order to build stronger ones
```
