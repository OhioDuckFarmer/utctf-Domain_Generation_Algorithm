# Write-up of UTCTF Challenge: Domain Generation Algorithm

Challenge   : Domain Generation Algorithm

Point Value : 400

Source Image: https://storage.googleapis.com/utctf/dga

Scenario    :  This executable calculates a new domain depending on the system time. See if you can predict what the new domain will be on Tue, 20 Apr 2021 13:25:03 GMT.

Note        : the flag is utflag{domain_name.tld}

Developer   : jitterbug_gang


Understanding what we are dealing with:

After downloading the binary the first thing I did was to confirm that I was working with an executable (after all, this is a CTF challenge and we can't just take the developers word for it).  For this I used the file command from within my Kali VM

root@kali:~/tmp# file dga
dga: ELF 64-bit LSB executable, x86-64, version 1 (SYSV), statically linked, no section header
