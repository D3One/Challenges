🔐 CRIMINAL CHALLENGE: Hunting for a botnet in AWS 🛡

Our case:  
Three of our servers in the AWS cloud turned into zombies. Hackers are using them for:  
💰 Cryptomining (XMRig)  
     ☠️ DDoS attacks on corporations  
    🎣 Phishing campaigns from legitimate IP addresses

😱 SOC specialists have given up — the rootkit masks processes, and the logs have been partially wiped.  We only have handmade tools, no forensic enterprise software or complex detection systems (SIEM, xDR, EUBA, etc.)

Your task, guys:  
1️⃣ Find the point of entry (how did they get in?)  
2️⃣ Reveal the persistence mechanisms  
3️⃣ Identify C2 channels  
4️⃣ Detect artifacts of malicious activity  (artifacts, indicators of compromise, traces)

Here's what we have for analysis:  
- iptables-save.txt - firewall rules  
- ps-aux-snapshot.txt - masked processes  
- netstat-tunap.txt - network connections  
- suspicious.pcap - traffic dump (text)  
⚠️ Additional files:  crontab(root), auth.log 

➡️ Format of your answer for it to be counted:  
- Indicators of compromise (IoC)  
- Kill Chain reconstruction  (how? where? in what sequence? using what?)
- Cleanup recommendations  (restore machines without reinstalling, backups/snapshots)

🏆 The best analysis will receive a one-year subscription to Telegram Premium

🔽Logs, dumps, and uploads can be found below🔽all files, except for *.TXT, open in PDF (for convenience)

#quiz