# Invoke-ADConnection Version 2 !

**Main Usage:** This tool doe's the same as [Invoke-ADConnection](https://github.com/7ysN/Invoke-ADConnection), but additionaly,
It's contains the Microsoft Active Directory Module DLL which is compressed and encoded to a Base64 string.
It's also checks the User's loggon attepmts before running, to ignore users from lockout.


## Usage:

1. `PS C:\Tmp> . .\Invoke-ADConnection_V2.ps1`
2. Users list will be generated and save as ` Users.txt `
3. Enter a ` password `. 
4. Results will be saved as ` UsersFound.txt `

![image](https://github.com/7ysN/Invoke-ADConnection_v2/assets/62604022/ebbf3eed-12cb-413c-a391-ec74d8a6ab8f)

## Further Steps:
After finding some users, you can use the tool: **[Active Directory Map](https://github.com/YuvalSab/Active-Directory-Map/blob/main/ActiveDirectoryMap.ps1)**
. This tool contains the Function **`UsersMembership`** that helps to map user's group membership

**`UsersMembership` Function:**

![image](https://github.com/7ysN/Invoke-ADConnection_v2/assets/62604022/741438ef-e115-4277-8f13-ee1c4843701d)
#
### Good Luck !
#
### Disclaimer

###### This tool is intended for educational and authorized security operations only. Unauthorized use of this tool may violate applicable laws and regulations. The developers and distributors of this tool assume no responsibility for any misuse or damage caused by its use. By using this tool, you agree to use it in compliance with all relevant laws and only for lawful purposes, such as cybersecurity research, penetration testing on systems you own or have explicit permission to test, and educational demonstrations. Unauthorized access to computer systems is illegal and unethical. Use this tool responsibly.
