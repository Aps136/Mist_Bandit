# Mist_Bandit
## BANDIT 0-1

### commands used:
ssh bandit0@bandit.labs.overthewire.org -p 2220
### when promted for password, write bandit0 
cat readme
### password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
exit


## BANDIT 1-2

### commands used:
ssh bandit1@bandit.labs.overthewire.org -p 2220
### ENTER password from prev level
cat ./-
### password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
exit

## BANDIT 2-3
### ssh bandit2@bandit.labs.overthewire.org -p 2220
### Enter password from prev level
### ls
### cat "spaces in this filename"
### password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
### exit

## BANDIT 3-4
### ssh bandit3@bandit.labs.overthewire.org -p 2220
### Enter password from prev level
### cd inhere
### ls -a
### find . -type f -name '.*'
### cat .hidden
### password obtained: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
### exit

## BANDIT 4-5
### ssh bandit4@bandit.labs.overthewire.org -p 2220
### Enter password from prev level
### command used:
### cd inhere
### ls
### file ./*  
### cat ./-file07
### password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
### exit

## BANDIT 5-6
### ssh bandit5@bandit.labs.overthewire.org -p 2220
### Enter prev level password
### command used: 
### cd inhere
### find . -type f -size 1033c ! -executable -exec file {} + | grep ASCII
### cat ./maybehere07/.file2
### password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
### exit

## BANDIT 6-7
### ssh bandit6@bandit.labs.overthewire.org -p 2220
### Use prev level password
### find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
### cat /var/lib/dpkg/info/bandit7.password
### password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
### exit

## BANDIT 7-8
### ssh bandit7@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### find / -name "data.txt" 2>/dev/null
### grep "millionth" ./data.txt
### password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
### exit

## BANDIT 8-9
### ssh bandit8@bandit.labs.overthewire.org -p 2220
### Use prev level password
### cat data.txt
### cat data.txt | sort | uniq -u
### password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
### exit



## BANDIT 9-10
### ssh bandit9@bandit.labs.overthewire.org -p 2220
### Use prev level password
### commands used: 
### ls
### sort data.txt | uniq -u
### password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
### exit



## BANDIT 10-11
### ssh bandit10@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### cat data.txt
### password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
### exit


## BANDIT 11-12
### ssh bandit11@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### cat data.txt
### cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
### password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
### exit


## BANDIT 12-13
### ssh bandit12@bandit.labs.overthewire.org -p 2220
### Use prev level password
cd $(mktemp -d)
cp ~/data.txt .
xxd -r data.txt binaryfile
file binaryfile

### mv binaryfile binaryfile.gz
gunzip binaryfile.gz
file binaryfile

### mv binaryfile binaryfile.bz2
bunzip2 binaryfile.bz2
file binaryfile

### mv binaryfile binaryfile.gz
gunzip binaryfile.gz
file binaryfile

### mv binaryfile binaryfile.tar
tar -xf binaryfile.tar
file binaryfile
ls -l
total 36
file data5.bin
mv data5.bin data5.tar
tar -xf data5.tar
ls -l
total 40
tar -xf data5.tar
ls -l
total 40

### file data6.bin
mv data6.bin data6.bz2
bunzip2 data6.bz2
ls -l
total 48

### file data6
mv data6 data6.tar
tar -xf data6.tar
ls -l
total 52

### file data8.bin
mv data8.bin data8.gz
gunzip data8.gz
ls -l
total 52

### file data8
data8: ASCII text
cat data8
### The password: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
exit

## BANDIT 13-14

### ssh bandit13@bandit.labs.overthewire.org -p 2220
### ls
### sshkey.private
### cat sshkey.private
### ssh -i sshkey.private bandit14@localhost -p 2220
### cat /etc/bandit_pass/bandit14
### password: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
### exit


## BANDIT 14-15
### ssh bandit14@bandit.labs.overthewire.org -p 2220
### commands used:
### telnet localhost 30000
### entered password 14
### PASSWORD: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
### exit


## BANDIT 15-16
### ssh bandit15@bandit.labs.overthewire.org -p 2220
### commands used: 
### openssl s_client -connect localhost:30001
### entered password 15eel1
### PASSWORD: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
### exit







