Programmer: Roberto Perez Mendoza
CPSC-456 Advanced Network Security
Fall 2018
Topic: Creating a worm using python 

1. Check if the current system contains a marker file (/tmp/marked.txt or something similar). If marked, then we are done.  If not, go on.
2. If not marked, use nmap in order to scan the local subnet. This will return the list of IPs of systems that are listening on port 22 (i.e., potential victims)
3. The worm goes through the list of systems and attempts a bruteforce attack by trying sets of user names and passwords from the dictionary. If the login succeeds, great! Go on!
4. Copy yourself to the system and execute! On the infected system the worm repeats the process from 1.