# Test-ADConnection Version 2 !

**This script contains the Microsoft Active Directory Module DLL which is compressed and encoded to a Base64 string.**
**This script performs a connectivity check against Active Directory LDAP Service.**
**The script generate a Users list of the current domain and tries to log in with the given password.**
**The script will only display users whose password is correct.**

## Usage:
`PS C:\Tmp> . .\Test-ADConnection_V2.ps1`

**The script first loads the Active-Directory Module.**
**The script then generates automatically a Users list and save it as `"Users.txt"` in the same folder from which it runs.**
**When it finishes creating a list of users, the script asks for a `password`. The script will then attempt to connect to the LDAP service for those users from the list:**

*The whole process is automatic except for entering the password.*
![2023-02-07 13_38_43-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217238210-350eddd1-f77a-41d0-8b1a-5080d716e2ba.png)

### The script counts how many users have been found, and shows it using a metric. This metric shows the running progress:
![2023-02-07 13_39_12-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217239625-6d90bac3-0e40-402f-94d6-e56456d4c6da.png)

### When the script finishes running, an additional file called `"UsersFound.txt"` will be created containing the users whose password is correct:
![2023-02-07 13_42_12-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217239650-acf33d7c-68b1-40bb-88cf-c78b7a38531d.png)

*Files Created:*

![2023-02-07 13_42_54-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217239660-ebb9c2d7-1ca6-4dbd-8223-1133e7188bab.png)
 

## Further Steps:
### After findings some users, you can use the following script:
**[Active Directory Map](https://github.com/YuvalSab/Active-Directory-Map/blob/main/ActiveDirectoryMap.ps1)**

**In this script there is the `UsersMembership` function that helps with checking the user's group membership !**


**`UsersMembership` function:**

![2023-02-07 14_36_18-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217247670-091a78da-35af-4fc8-b9bf-7fef38d0fe52.png)

**Entering a wordlist - in our case `UsersFound.txt`:**

![2023-02-07 14_36_57-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217247841-1fdf6fda-dbdf-44ed-9a56-a7d49fee1ea2.png)

**The Results:**

![2023-02-07 14_37_44-win10 (win10 clear)  Running  - Oracle VM VirtualBox](https://user-images.githubusercontent.com/62604022/217247966-7fcefa46-2550-4cef-b965-9322e10564c7.png)


## Good Luck !
