:pushpin: :pushpin: :pushpin: Replicated from https://github.com/eddiechu/Encrypt-Delete-Test :pushpin: :pushpin: :pushpin: 

# Really can protect from ransomware encryption?

We often come across antivirus and next-generation endpoint solutions that claim to offer ransomware protection, boasting advanced capabilities in detecting activities such as penetration, invasion, and pre-encryption through the use of AI and machine learning. However, these solutions may still fail to prevent the encryption process if they happen to miss detecting these malicious activities.

To address this concern, we have developed a simple tool that simulates the ransomware encryption process. This tool can help you determine whether your EDR (Endpoint Detection and Response) or antivirus software is capable of blocking such malware encryption behaviors.


[![Watch the video](https://raw.githubusercontent.com/eddiechu/Powershell-ransomware-simulator/main/Image/mr.bean2.gif)](https://youtu.be/CQIq8GDtDG0)

**Stop encryption is the last defense, which cannot be neglected.**


# Which brand can detect encryption operation?

That's why I developed this tool.  It is not to replicate found malware, not vendor test tool, no bias, no need to install, just do **encrypt (in memory) - overwrite (original file) - rename (file extension)**, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

I have helped people to test this after WannaCry outbreak.  Luckly, I found few brands can detect it, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  I did see a real Ransomware incident, that endpoint really could stop encryption, no loss.

You can refer to the source code if you know programming or you can download the complied files.

Hope there is no more ransomware incident!  Please share this blog with friends if you found it is useful.


# This tool

Please copy and paste the PowerShell code to terminal, this way can bypass antivirus signature and simulate the real ransomware behaviour



![alt text](https://raw.githubusercontent.com/eddiechu/Powershell-ransomware-simulator/main/Image/powershell1.gif)

This tool encrypts - overwrite - rename the files in the selected (local or network) folder and subfolder, you may create a temporary folder like C:\Ransomware-Simulator\, save this tool to there, then run it.  Be safe.

It tests if your endpoint can detect when encryption is happening (like base on the files change pattern), but NOT to test if your endpoint can prevent it from start.

It is great if you can share your test result with me for my record.







#

ransomware test tool
ransomware simulation
ransomware simulator
ransomware assessment
eddie chu
eddiechu.android@gmail.com
anti-ransomware
antivirus test
anti-virus test
endpoint test
infosec
security
cyber security
cybersecurity
incident response
hacker
antimalware
anti-malware
encryption
encrypt-del-test
encrypt-delete-test
encryptdeltest
encrypt overwrite rename
tool
test tool
defense
testing
pentest
penetration test
blue team
red team
poc
ciso
