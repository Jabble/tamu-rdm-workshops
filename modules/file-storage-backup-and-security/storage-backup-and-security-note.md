# Storage, backup, and security
## 2. Introduction
In this module, we'll focus on storage of digital data. 
We'll cover:

- storage locations, 
- and discuss data backup and security. 

The goal is to think "safety first" and reduce risks.

## 3. What risks?
We'll focus on reducing the likelihood of:

- Data loss
- File corruption
- Unauthorized data access

**Data loss** may occur if a file is accidentally deleted, a computer is stolen, or a hard drive fails and data are not backed up. 

**File corruption** may occur when digital files are moved or copied, and when they are stored on one medium for a long period of time. 

**Unauthorized access** may occur if appropriate security precautions are not followed for sensitive data.

## 4. Discussion: Choosing storage and back up locations
*Group discussion, taking live notes for each storage location*

The location of your data will likely depend on the degree of freedom you have in the management of your data. Your data may need to be stored in a particular location due to legal and ethical considerations, or due to your lab or research group's practices. 

In this section we will survey 4 types of storage locations, discussing features that help to assess the benefits and risks of using particular locations for storing and backing up your data.

We'll talk about:

- Accessibility
- Space
- Security
- Integrity

### 5. Personal computers
#### Accessibility
- Convenient for storing data while in use.
#### Space
- Limited to space available on the computer hard drive.
#### Security
- Can be lost or stolen.
- Can have multiple valid users with access.
- Hard drive may or may not be encrypted.
#### Integrity
- Files are stored on the local hard drive, which will eventually fail.
- Depends on personal practices for:
	- Regular backup to another location.
	- Software updates.

### 6. Personal computers
- Recommended for working with data that aren't sensitive or restricted.
- Depend heavily on personal practices.

### 7. External hard drives or USB sticks
#### Accessibility
- Low cost
- Portable, can be kept locally and attached to personal or work computers
#### Available space
- Same scale as personal computers, limited to space available on the hard drive or USB stick.
#### Security
- May easily be lost or stolen.
- Hard drive or USB stick may or may not be encrypted.
#### Integrity
- USB sticks are flimsy.
- External hard drives will eventually fail.

### 8. External hard drives or USB sticks
- Usually used as a location for backup or for data sharing.
- Depend heavily on personal practices.

### 9. University networked drives
central it provides storage for departments, typically at the dept. level. Looking at options to give access.
#### Accessibility
- Made accessible via log in on personal or work computer.
#### Available space
- Depends on agreement with IT, may have a cost.
- Capable of storing large datasets.
#### Security
- Access controlled by IT staff.
- Measures may be set up for storing sensitive and controlled data.
#### Integrity
- Storage is distributed, with redundancy for failure of a single hard drive.
- Regular update and back-up strategies are in place.

### 10. University networked drives
- Recommended for storing master copies of data.
- Managed by professional IT staff.

### 11. Third-party services
**TAMU-sponsored services:**

- TAMU Google Drive
- Syncplicity

**Other common services:**

- Amazon S3 ("cloud" computing storage facilities)
- Dropbox
- SpiderOak

### 12. Third-party services
#### Accessibility
- Accessible via log in, usually via web browser or a computer application.
- Store files remotely and synchronise files across local computers.
- Most are platform-agnostic.
#### Available space
- Usually provide the first few gigabytes free and users pay for more space.
- Capable of storing large datasets.
#### Security
- Depends on the service.
- Some services may have measures for storing sensitive and controlled data.
- Services operated on servers physically located outside US may be a problem for some data.
#### Integrity
- Usually provide versioning, but this may be limited.
- Storage is distributed, redundancy for failure of a single hard drive.
- Regular update and back-up strategies are in place.
- Service provider may go out of business.

### 13. Third-party services
- Recommended for sharing with collaborators and for working data.
- These services store and synchronize data files and offer redundant backup services for users.
- Be sure to read the fine print and not only rely on commercial options for storing your data.
	- They may use banks of servers located around the globe, which might not be allowed with yout data.
	- Commercial cloud storage and sharing services may have size, cost, or privacy limitations that could pose a risk to your data.  
	- Commercial web applications can be discontinued unexpectedly, and you will want to know what happens to your data in that scenario.  

You want to know details about privacy and about:

- how much storage you have, 
- for how long, 
- and for how much money.

## TAMU-sponsored online services
### 14. Google Drive
- **Google Drive** is a cloud storage service that allows you to store an unlimited amount of files that you can access anywhere you have an internet connection. 
	- You can upload documents, presentations, pictures, videos and anything else you may need.
- **Google Team Drive** is a new addition similar to Google Drive, but is especially designed for teams. 
	- Files in Google Team Drive belong to the team instead of an individual user, so shared files remain even if a member leaves.

- Users of the Service must follow both Google’s Acceptable Use Policy and Texas A&M University IT Security Controls.

**The Service is not appropriate for:**

- Electronic Protected Health Information (EPHI) subject to the Health Insurance Portability and Accountability Act (HIPAA).
- Data controlled for export under Export Control Laws (EAR, ITAR).
- Certain types of Personally Identifiable Information (PII), including Social Security Numbers, credit card numbers, and bank or financial account numbers.
- High Risk Activities such as those involving business records in which loss or inappropriate disclosure would result in large consequences in terms of economic loss, loss of trust, or legal liability.

Data Sharing: Users of the Service can allow others to access data for the purpose of sharing and collaboration. 

Do not share data with anyone who does not have the appropriate authority to view it unless the data is of a public nature.

Google Apps at Texas A&M. "Terms Of Use and Privacy" [website](http://google.tamu.edu/Resources/terms_of_use.html)

### 15. Syncplicity
Syncplicity offers a secure cloud environment for users in The Texas A&M University System to store documents. 

Your department has to buy in, so you may need to check if it is available.

Offers users the ability to sync any folder or desktop, include and exclude subfolders, and use native clients for Windows, Mac, iOS, and Android.

TAMU IT [website](https://tamu.service-now.com/tamu-selfservice/knowledge_detail.do?sysparm_document_key=kb_knowledge,267fe85c6f985a400798122cbb3ee4e0)

## 16. Exercise: Thinking about storage
- Where do you think you will you store your data?
- How many copies of your data will you keep?

## 17. Storing data
Good practices for storing data to reduce the likelihood of data loss and file corruption.

1. Keep at least 3 copies of data in at least 2 geographically distributed locations. 
- Original 
- External backup, kept locally 
- External backup, kept at a remote location

For storage that you control, redundancy is an integral part of data management. Geographically distributed copies reduce the risk posed by a calamity at one location. You can think of it as insurance in case of theft, power outage, flood, fire, etc.

2. Check data integrity after copying data files, and regularly check backup files.
- Restore your data files from backups to check that they can be read
- Generate checksums

Digital files can be corrupted when they are copied, moved, or stored for a long period.

3. Copy data files to new media 2–5 years after first created.

All storage media (e.g. hard drives) break down over time. 

## 18. Create a backup system
- Backup allows you to restore your data in the event that it is lost.
- Backup is important for all data, but particularly for research data that is unique or difficult to reproduce.
- The aim with a backup system is to manage multiple copies and keeping them up to date

Your strategy will depend on:

- the amount of data you are working with, 
	- Your strategy should be able to accommodate the amount of data that you anticipate collecting and be stable for the length of time that you anticipate keeping your data. 
- the frequency that your data changes,
- and the system requirements for storing and rendering it. 

These are some questions that can guide you:

1. How much space will you need to store your original data?
	- How large are your data files?
	- Is your data collection iterative?
	- How much data will you accumluate every day, week, or month?
	- How much data do you anticipate collecting and generating by the end of your project?

2. How often will backups be made?
	- Think about how often you make changes to the data.
	- Common schedules are daily, weekly, or monthly.
	- If you are making frequent or important changes to your data, you should backup your files on a daily basis. 
	- If you modify your data files less frequently, a longer backup schedule – weekly or monthly – may be sufficient. 


3. How do you want to back up your data?
	- Will all the data be backed up each time (full backup), or only amended data and changes (incremental backup)?
	- A **full backup** will replicate all the files on your computer. Full backups take a long time and require the most storage space. 
	- **Differential incremental backup** copies only those files that have changed since the last incremental or full backup.

4. How long will each backup be stored before being over-written? 
	- For example: under the Grandfather-Father-Son rotation scheme, files may be available for two to three months before the space is over-written.

5. How much additional space will be required to maintain the backups?
	- Think about your answers to the questions above to help you estimate.

6. Where will you backup your data locally? And remotely?
	- Which hardware and services are available that meet your accessibility, security, and space needs?
	- If you are working from a networked computer, your IT division likely has a backup protocol in place. Contact your IT department for their backup plan. 
	
7. How will you keep track of different versions of data when backing up to multiple devices? 
	- Will you use a Version Control Systems (VCS)?

## 19. Software can help
Once you have an idea of what you want. 

You can choose to schedule and regularly copy files over to your storage locations and manage versions.

Or, you can use Software that automatically backs up files to automate and simplify the process. 

These software tools can backup to the locations you choose, at the schedule you choose.

- Time Machine: Mac-only, application distributed with the Apple operating system.
	- The software works with internal and external disk drives. 
	- Creates incremental backups of files that can be restored at a later date
	- Time Machine saves hourly backups for the past 24 hours, daily backups for the past month, and weekly backups for everything older than a month until the volume runs out of space. 
	- At that point, Time Machine deletes the oldest weekly backup.

- Arq: Mac, Windows ([website](https://www.arqbackup.com))
	- Allows you to store encrypted backups with cloud services, or network attached storage. 
		- You pay for your own storage
	- Backups are versioned.
	- Can backup your computer and external drives too.
	- You can choose to backup whole drive of certain files.
	- You can set back up size limit and deletion rules. 

- Backblaze: Mac, Windows ([website](https://www.backblaze.com/cloud-backup.html))
	- Online backup software with storage solution (monthly price)
	- Allows you to store encrypted backups to their datacenters storage.
	- Aimed at ease of use. Similar approach as Time Machine and backing up all user data.
	- Allow for two-factor authentication.
	
*Show one*

## 20. Test backups
To be sure that your backup system is working, periodically retrieve your data files and confirm that you can read them. 

You should do this when you initially set up the system and on a regular schedule thereafter.

Any questions about backups?

## 22. Security tips
We're going to move on to talk a little about security.

As we discussed in the "Legal and ethical considerations" module, if you're working with sensitive or restricted data, you're responsible for maintaining confidentiality of identifiable data and security.

This means:
 
- data on your computer may need to be kept safe. 
- Or you may be given access to a secure system that stores the data. 

Make sure to work with your advisor and your research team to understand and meet data security requirements. 

General good practices to reduce the likelihood of unauthorized data access for 

- sensitive and restricted data, 
- or data that you don't want to share:

- Be aware of policies for moving or sharing the data.
	- Speak with your advisor.
- Avoid logging in to secure spaces using untrusted computers or networks.
	- Such as café wifi.
	- If you do log in, use a Virtual Private Network (VPN)
- Make sure physical storage media are in a locked room or safe
	- Lock up your computer or hard drives when they are not in use.
	- Servers managed by the university or third parties should also be located in secure rooms.
- Use strong passwords and be careful with your login credentials.
- Store and transmit sensitive data using encryption.
- Ensure complete destruction when deleting sensitive data.

## 23. Passwords 
Strong passwords are important to maintaining security against attacks that are aimed at guessing passwords to gain access to user accounts. 

These attacks are clever and a few tips can save you a lot of trouble. 

Tips:

- Create unique passwords for your accounts
- Use 18 or more characters where possible, and max it out if you can
- Use nonsense "passphrases" with fake words, numbers, and symbols

Does anyone use a password management software?

A password manager is another software that can can make your digital life significantly easier and more secure:

- 1password
- LastPass

Basically, these software tools encrypt and store your account information, including userid and passwords,  on your computer for you. 

- They offer additional features to generate strong passwords for you,
- and auto-fill your account information in browser windows.
- They can also be used to store other information like passport details and secure notes.

## 24. Discussion
Does having a password protect you data if your computer is stolen?

### Fun fact: Login passwords on your computer are easy to bypass
Your computer password doesn't necessarily keep your data safe. 

Unless your files are encrypted on your computer, someone who has physical access to your computer can get access to your data with enough effort.

How? Basically, your computer's hard drive can be used like a big USB stick. 

- File permissions for a user are set by your operting system. 
- If someone boots your hard drive with their operating system, those permissions are irrelevant. 
- This can involve different strategies for Macs and PCs, but in both cases it's easy to do with a bit of effort.

As a precaution, encypt your hard drive.

Find out More: 

- PC example: hard drive taken out of computer and mounted on another host gives them access. 
- Mac example: Connecting your Mac to another Mac and booting your Mac in Target Disk Mode, your Mac's hard drive will appear as a mounted drive on the other Mac. Unless Mac1 is encrypted with FileVault, all files will be accessible [website](https://support.apple.com/kb/PH10725?locale=en_US)

## 25. Encryption
Encryption is the process of converting data into an unreadable code. You must have access to a password or a secret encryption key to be able to read an encrypted file.

Encrypting your data will help ensure your data remain safe from disclosure in the event that a laptop, desktop, USB stick, or external hard drive are lost or stolen. 

Still, data encryption is not a substitute for other information protection controls. 

- It still relies on the creation of a strong password. 
- If the encryption key is lost, the disk image gets corrupted, or the hard disk fails, any encrypted data will be lost.

You should use mainstream encryption tools. TAMU IT recommends:

- Bitlocker: is a whole disk encryption included in Windows Vista and later.
- FileVault: is a built-in tool on Macs for whole disk encryption.

**Data files on computer**
You can encrypt individual files or folders on your computer.

**Entire computer hard drive or USB stick**

software:

- BitLocker: Windows full disk encryption
- FileVault: Mac

### Files in transit
Files in transit should also be protected.

TAMU IT recommends not to send files through email:

- Filex: provides a secure and easy-to-use file distribution system. 
	- It has a single-click encryption option for files that contain confidential or sensitive information. 
	- Go to filex.tamu.edu to use the system.
	
If you want to get more into it.

- Pretty Good Privacy (PGP) PGP (also known as OpenPGP) is a standard for making methods of encryption and decryption easily available for public use. 
- PGP provides cryptographic privacy and authentication for data communication.
- GNU Privacy Guard (GPG) is a full implementation of the OpenPGP framework. 
	- Find out more: https://gnupg.org
- GPG based programs can encrypt files, folders, and emails.
- A couple of user firenldy programs recommended by TAMU IT include:

- Gpg4win: Windows
- GPG Suite: Mac OS

### VPN
If you do access a page that requires a login and password, make sure the web site uses "https" not just "http."


It provides increased security by encrypting all data sent to and from your computer, useful when using insecure wifi networks. 
Using a VPN is especially important when visiting websites that contain confidential information, such as banking websites.


- Virtual Private Networking (VPN) is a method of providing a more secure network connection from public or untrusted networks. 
- When a VPN connection is established, it creates an encrypted communication path between your computer and the VPN server. 
- This helps to protect your network traffic from many types of common network attacks, which could be used to expose confidential information. 

AnyConnect VPN client
https://tamu.service-now.com/tamu-selfservice/knowledge_detail.do?sysparm_document_key=kb_knowledge,02ce68792badc6009b4c26e405da151e

Because the VPN server is hosted within the Texas A&M University firewall, a VPN connection will also provide access to university resources that are not typically available from non-TAMU connections.


### Sentitive Data Deletion
File deletion is not enough to ensure that sensitive electronic data are completely removed from a computer system. File deletion removes only the pointers to the disk sectors in which the data reside. 

Deleted files can be recovered using commonly available software tools.

To ensure the complete destruction of sensitive data, the main options are:

- Data erasure, also called "data clearing" or "data wiping." This involves using software to remove all data by overwritting it. It leaves the hard drive or other storage medium operable.
- Degaussing. This disturbs the magnetic alignment of magnetic storage media and in many cases makes newer media, such as hard drives, unusable.
- Physical destruction. Through disintegration, shredding, pulverizing or incineration.

## Conclusion
- Review risks associated with data storage
- Discuss data back up
	- Keeping backups is an essential data management task. 
	- There is a real risk of losing data through hard drive failure or accidental deletion. 
	- Recommended that you keep at least 3 copies of your data on at least 2 different media, keeping storage devices in separate locations with at least 1 off-site, and check that they work regularly.
	- You should also have a policy for maintaining regular backups.
- Identify tools and strategies for keeping data secure

## Bonus
- Before the next session, ask your advisor where he/she stores his/her data and how it's backed up
- If they use network drives, who manages them and do they know the security and backup policies?

## References
- DMPTool. "Data Management General Guidance" [Website](https://dmptool.org/dm_guidance)
- Google Apps at Texas A&M. "Terms Of Use and Privacy" [Website](http://google.tamu.edu/Resources/terms_of_use.html)
- Hicock, Robyn. 2016. "Microsoft Password Guidance" [PDF](https://www.microsoft.com/en-us/research/publication/password-guidance/)
- MANTRA. "Storage and security" [Module](http://mantra.edina.ac.uk/storageandsecurity/)
- New England Collaborative Data Management Curriculum. "Module 4: Data Storage, Backup, and Security" [Website](http://library.umassmed.edu/necdmc/modules)
- TAMU. "Protecting Confidential Information" [Website](https://security.tamu.edu/protect_my_work/Protecting_Confidential_Information.php)
- TAMU. "SAP29.01.03.M1.16: Information Resources — Portable Devices: Information Security"[PDF](http://rules-saps.tamu.edu/PDFs/29.01.03.M1.16.pdf)

## Materials
### Handout
*Physical handout and available online for download*

Questions to guide a storage and backup strategy:

1. How much space will you need to store your original data?
	- How large are your data files?
	- Is your data collection iterative?
	- How much data will you accumluate every day, week, or month?
	- How much data do you anticipate collecting and generating by the end of your project?

2. How often will backups be made?
	- Think about how often you make changes to the data.
	- Common schedules are daily, weekly, or monthly.
	- If you are making frequent or important changes to your data, you should backup your files on a daily basis. 
	- If you modify your data files less frequently, a longer backup schedule – weekly or monthly – may be sufficient. 


3. How do you want to back up your data?
	- Will all the data be backed up each time (full backup), or only amended data and changes (incremental backup)?
	- A **full backup** will replicate all the files on your computer. Full backups take a long time and require the most storage space. 
	- **Differential incremental backup** copies only those files that have changed since the last incremental or full backup.

4. How long will each backup be stored before being over-written? 
	- For example: under the Grandfather-Father-Son rotation scheme, files may be available for two to three months before the space is over-written.

5. How much additional space will be required to maintain the backups?
	- Think about your answers to the questions above to help you estimate.

6. Where will you backup your data locally? And remotely?
	- Which hardware and services are available that meet your accessibility, security, and space needs?
	- If you are working from a networked computer, your IT division likely has a backup protocol in place. Contact your IT department for their backup plan. 
	
7. How will you keep track of different versions of data when backing up to multiple devices? 
	- Will you use a Version Control Systems (VCS)?
	
Software list:
