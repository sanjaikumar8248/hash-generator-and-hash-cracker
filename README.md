# sanhasher
This Tool will generate a live hash of your Password/Text, and will generate a hashes of your Files, and verify the password or text can be easily cracked by verifying it in the dictionary of wordlists.......
Menu:
1. Password Hash Generator
2. File Hash Generator
3. Password Hash Checker
99. Exit

This project demonstrates:
- Password/text hashing
- File integrity hashing
- Dictionary-based password strength checking

How to use:
- command: python3 sanhasher.py

Use your wordlists to crack or use a sample wordlist to do sample checking.....

Educational & offline use only.













exper= 1 (Cyber Security Fundamentals for Forensic Investigation)


nano evi.txt

sha256sum evi.txt

 stat evi.txt


rm evi.txt


ls -la


exper= 2 (FAT32 File systems - History and background on FAT - Allocation Tables -
Directory Entries - Bitmaps - Deleted files and unallocated space)


dd if=/dev/zero of=fat32.img bs=1M count=20


mkfs.fat -F 32 fat32.img


mkdir /mnt/fat32
mount fat32.img /mnt/fat32


cd /mnt/fat32
 echo "FAT32 Forensic Practical" | sudo tee  file1.txt
 echo "Cyber Forensics" | sudo tee  file2.txt
ls


stat file1.txt


rm file1.txt
ls

fsck.fat -v fat32.img


umount /mnt/fat32

exper=3. (NTFS File Systems - History & background of NTFS - Master File Table
(MFT) - MFT Entries - Deleted Entries - Unallocated space)




dd if=/dev/zero of=ntfs.img bs=1M count=30


mkfs.ntfs ntfs.img


mkdir /mnt/ntfs
mount ntfs.img /mnt/ntfs


cd /mnt/ntfs
sudo echo "NTFS Forensic Practical" | sudo tee  file1.txt
sudo echo "MFT Analysis" | sudo tee  file2.txt
ls


stat file1.txt


rm file1.txt
ls


ntfsinfo -m ntfs.img


umount /mnt/ntfs


exper=4. (File sharing–File sharing logs - Network logs - Advanced BitTorrent
Analysis)



cd /var/log
ls


cat auth.log


netstat -ant


ip a


 6881 – 6889
netstat -an | grep 688


sudo apt install transmission-cli


transmission-cli example.torrent


netstat -ant | grep ESTABLISHED


exper=5.  (Executable File Analysis - Static Analysis - Dynamic Analysis –
Virtualization)



file sample.exe


sha256sum sample.exe


strings sample.exe


objdump -x sample.exe


ls -lh sample.exe


PART B: DYNAMIC ANALYSIS


chmod +x sample.exe
./sample.exe





exper=6.   (Email and Internet Analysis - Web cache, history, bookmarks - Mail header
analysis - Email server analysis - Building timelines)



PART A: INTERNET ANALYSIS

C:\Users\Username\AppData\Local\Google\Chrome\User Data\Default\Cache

Press Ctrl + Shift + O


PART B: EMAIL ANALYSIS
Email Header Analysis
Step1:
 Open Email
 Click More options → View Original / Show Headers
Step2: Check Important Fields
From:
To:
Date:
Received:
Message-ID:
PART C: TIMELINE BUILDING


exper=7 (Windows Registry - Registry locations - Windows registry keys and values -
Useful registry keys - Automated tools for registry analysis)



Win + R → regedit → Enter


HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Winlogon


HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall


HKCU\Software\Microsoft\Windows\CurrentVersion\Run


HKCU\Software\Microsoft\Windows\CurrentVersion\Explorer\RecentDocs


Tool 2: RegRipper

 rip.exe -r NTUSER.DAT -f ntuser

exper=8 (Network forensics analysis using “Xplico “.)




sudo apt update
sudo apt install xplico -y


sudo xplico start


Ip a


xplico -m case -n Network_Forensics


xplico -m session -c Network_Forensics -n Session1


xplico -i eth0 -c Network_Forensics -s Session1


ping google.com


CTRL + C


http://127.0.0.1:9876
 Username: xplico
 Password: xplico




full notes pdf guysssssss

https://drive.google.com/file/d/134HsoVJjCTCPo--1Carep7UuGjvTBDR0/view

