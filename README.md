# Mist_Bandit
## BANDIT 0-1
![bandit0](https://github.com/user-attachments/assets/2e19b64f-47b8-4ac5-bed3-23972f09883d)


### commands used:
ssh bandit0@bandit.labs.overthewire.org -p 2220
### when promted for password, write bandit0 
cat readme
### password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
exit


## BANDIT 1-2
![bandit1-2](https://github.com/user-attachments/assets/d43e8c5a-ec44-4ef2-a4f6-d3c21730d77e)



### commands used:
ssh bandit1@bandit.labs.overthewire.org -p 2220
### ENTER password from prev level
cat ./-
### password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
exit

## BANDIT 2-3
![bandit2-3](https://github.com/user-attachments/assets/fbe05547-7785-4ce1-a648-449f5be8032b)


### ssh bandit2@bandit.labs.overthewire.org -p 2220
### Enter password from prev level
### ls
### cat "spaces in this filename"
### password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
### exit

## BANDIT 3-4
![badnit3-4](https://github.com/user-attachments/assets/41af7898-e7d5-4608-8ebd-722b69d544df)


### ssh bandit3@bandit.labs.overthewire.org -p 2220
### Enter password from prev level
### cd inhere
### ls -a
### find . -type f -name '.*'
### cat ...Hiding-From-You
### password obtained: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
### exit

## BANDIT 4-5
![badnit5](https://github.com/user-attachments/assets/368dcff8-9bf4-4561-acc9-825fada4bb7d)

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

![bandit6](https://github.com/user-attachments/assets/28445692-9254-4f29-ada7-a9b7ea145144)
### ssh bandit5@bandit.labs.overthewire.org -p 2220
### Enter prev level password
### command used: 
### cd inhere
### find . -type f -size 1033c ! -executable -exec file {} + | grep ASCII
### cat ./maybehere07/.file2
### password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
### exit

## BANDIT 6-7

![bandit7](https://github.com/user-attachments/assets/b01d2221-34b1-4ea2-8d57-0c94de54ed9d)

### ssh bandit6@bandit.labs.overthewire.org -p 2220
### Use prev level password
### find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
### cat /var/lib/dpkg/info/bandit7.password
### password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
### exit

## BANDIT 7-8
![bandit7-8](https://github.com/user-attachments/assets/1dc4f841-9f4a-48ce-8470-b77e0938330e)

### ssh bandit7@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### find / -name "data.txt" 2>/dev/null
### grep "millionth" ./data.txt
### password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
### exit

## BANDIT 8-9
![bandti8-9](https://github.com/user-attachments/assets/740090d1-8448-4762-a67f-3b43c7d156fd)


### ssh bandit8@bandit.labs.overthewire.org -p 2220
### Use prev level password
### cat data.txt
### cat data.txt | sort | uniq -u
### password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
### exit



## BANDIT 9-10
![bandit9-10](https://github.com/user-attachments/assets/0e1f6bc3-0603-4f94-82d5-fe869111fbc7)


### ssh bandit9@bandit.labs.overthewire.org -p 2220
### Use prev level password
### commands used: 
### ls
### strings data.txt
### strings data.txt | grep '=='
### password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
### exit



## BANDIT 10-11

![badnit9-10](https://github.com/user-attachments/assets/38c0938d-0911-4eca-aca0-408bd76401c2)

### ssh bandit10@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### cat data.txt
### password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
### exit


## BANDIT 11-12
![badnit11-12](https://github.com/user-attachments/assets/faec6eaa-111c-4af1-ab8f-87763ffe1fc5)

### ssh bandit11@bandit.labs.overthewire.org -p 2220
### Use prev level password
### ls
### cat data.txt
### cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
### password: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
### exit


## BANDIT 12-13
![bandit13](https://github.com/user-attachments/assets/1105bde0-13cd-458a-9c2b-ea49c0d72447)


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
![p3](https://github.com/user-attachments/assets/57faadcb-645d-4c51-89e0-ccb372d5bb6a)

### ssh bandit13@bandit.labs.overthewire.org -p 2220
### ls
### cat sshkey.private
### ssh -i sshkey.private bandit14@localhost -p 2220
### cat /etc/bandit_pass/bandit14
### password: MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS
### exit


## BANDIT 14-15
![14-15](https://github.com/user-attachments/assets/24ccae87-64bc-48b1-8dfb-168a1f4c0050)


### ssh bandit14@bandit.labs.overthewire.org -p 2220
### commands used:
### telnet localhost 30000
### Enter prev password
### PASSWORD: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
### exit


## BANDIT 15-16
![15-6](https://github.com/user-attachments/assets/7decf2a7-a9bf-4bc3-815a-cb931850eda9)


### ssh bandit15@bandit.labs.overthewire.org -p 2220
### commands used: 
### openssl s_client -connect localhost:30001
### entered password prev password
### PASSWORD: kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx
### exit







