
Friends, here is the answer to our LINUX HACK QUIZ: FIND 5 FATAL ERRORS IN SUDOERS (https://t.me/w2hack/7469)

Thank you to everyone who participated, who tried their hand at it, even if they made mistakes, but didn't lose their enthusiasm👑 All versions were interesting, especially the one about the non-standard use of nmap (https://telegra.ph/ nmap-v-praktike-pen-testa-ot-enumeration-do-analiza-CVE-06-18) and its scripting engine (https://serverfault.com/questions/130946/is-it-dangerous-to-allow-every-user-to-run-nmap-as-root)🔥 Given that it is practically impossible to verify the accuracy of the answers (without AI and tricks) and the post was up for a long time, we do not have a single clear winner. There will be more contests and tasks ahead!🤝

⚠️ Here are the key security issues: ⚠️

📌 Error 1: NOPASSWD for /usr/bin/apt ➡️ installation of malicious packages without a password
📌 Error 2: NOPASSWD for /bin/chmod ➡️ changing permissions on any files (e.g., chmod 777 /etc/shadow)
📌 Error 3: NOPASSWD for /usr/bin/wget ➡️ downloading and running shell code
📌 Error 4: NOPASSWD: /bin/bash ➡️ risk of obtaining root shell without a password
📌 Error 5: NOPASSWD: /usr/bin/chattr -i /etc/passwd ➡️ removing protection from /etc/passwd to replace existing passwords

❓How to fix it:❓

# Require password entry
user1  ALL=(ALL) PASSWD: /usr/bin/apt 
# Disable bash!
%admin ALL=(ALL) /usr/bin/nmap 
# Remove chattr and wget from sudo!

⚡️ Bonus command: 
sudo visudo -c

This is all the basics for a young pentester, which will come in handy in CTF and solving challenges like HTB (junior