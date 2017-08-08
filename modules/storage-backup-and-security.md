# Storage, backup, and security
##Objectives
- Understand risks associated with storage lications where data files are stored and risks
- Design a storage strategy

## Introduction
Plan management -> **Collect and store** -> **Assure quality** -> Analyze and present -> Share and preserve

In this module, we'll focus on digital data storage, including locations and methods to back up data. The goal is safety first, to reduce the risk of data loss and security incidents.

## Storage space
Space is important to keep in mind when thinking about your storage and back up strategy. To avoid being under-prepared, estimate the growth rate of your data: 

- Are you manually collecting and recording data?
- Are you using observational instruments and computers to collect data?
- Is your data collection highly iterative?
- How much data will you accumluate every day, week, or month?
- How much data do you anticipate collecting and generating by the end of your project?

For instance, image data typically requires a lot of storage space. You may need to decide whether to retain all your images over the course of your research, and after your project is complete. 

## Data storage
Good practice:

Keep at least 3 copies of data in at least 2 geographically distributed locations. Geographically distributed copies reduce risk posed by a calamity at one location power outage, flood, fire, etc.)
Original + external backup located locally + external backup at a remote location

## Storage locations and maintenance
Storage locations will likely depend on how much freedom you have in the management of your data. Your data may need to be stored in a particular location due to legal and ethical considerations, or simply due to your lab or research group's practices. This section will point out features of different storage locations that may be useful to consider when using particular storage locations.





Space
Security
Accessibility
Integrity of back ups and storage media
Maintenance and update strategy

### Personal computer hard drive
#### Accessibility
- Convenient for storing your data while in use. Not recommended for storing master copies of data.

#### Space
- Limited to space available on your computer hard drive, on the range of 250 GB – 1TB

#### Security
- PCs and laptops may be lost or stolen
- May have multiple valid users
- Encryption

#### Integrity of storage media
- All content stored on the local drive, which may fail 

#### Back-up maintenance
- Depends on you


### External storage devices
External storage devices such as hard drives, USB flash drives (also known as memory sticks, USB keyrings or pen drives), Compact Discs (CDs) and Digital Video Discs (DVDs), can be an attractive option for storing your data due to their low cost and portability. However, they are not recommended for the long term storage of your data

#### USB stick, CDs, DVDs

#### External harddrive 
#### Back-up maintenance
- Depends on you


### University networked drives
Networked drives are managed by IT staff. 

#### Space
- 
#### Security
- 
#### Accessibility
- Access controlled by IT staff.
#### Integrity of storage media
- Storage is distributed, redundancy for failure of a single hard drive
- Depends on IT staff to perform and check integrity.

#### Back-up
- Regular back-up strategy in place. 

### Cloud servers

## Back up strategies


Making regular backups is an integral part of data management. You can backup data to your personal computer, external hard drives, or departmental or university servers. Software that makes backups for you automatically can simplify this process considerably. CDs or DVDs are not recommended because they are easily lost, decay rapidly, and fail frequently.

- Use a Cloud server as a sort of back-up and storage space accessible from multiple locations.

When considering your backup strategy you need to know:
	•	How will you back up your data?
	•	
	•	Will all data, or only amended data, be backed up? (A backup of amended data is known as an "incremental backup", while a backup of all data is known as a "full backup").
	•	
	•	How often will full and incremental backups be made?
	•	
	•	• How long will backups be stored? It is important to ascertain the back-up schedule and retention policies of any centralised backup services (e.g. under the Grandfather-Father-Son rotation scheme, files may be available for two to three months before the space is over-written).
	•	
	•	How much hard drive space or how many CDs/DVDs will be required to maintain this backup schedule?
	•	
	•	How will you keep track of different versions of data, especially when backing-up to multiple devices? If using versioning software, which software will you use (e.g., Tortoise, Subversion)?
	•	
	•	If the data are sensitive, how will they be stored securely and appropriately, and how will you manage the destruction of identifying data if required (e.g. at the end of your research)?
	•	
	•	What backup services are available that meet these needs and, if none, what alternatives are available?

Important! To ensure that your backup system is working properly, you should regularly test it by restoring your data files from your backups to check that you can read them.

Backing up data with Professor Richard Rodger,  University of Edinburgh [youtube](https://www.youtube.com/watch?v=jX-XNo8KbOo)

Remote, online or managed backup services provide users with an online system for storing and backing up computer files.

Typically online backup services:
	•	
	•	Allow users to store and synchronise data files online and between computers.
	•	
	•	Employ cloud computing storage facilities (e.g. Amazon S3).
	•	
	•	Provide the first few gigabytes free and users pay for more facilities, including space.

Wikipedia has a thorough comparison of online backup services: http://en.wikipedia.org/wiki/Comparison_of_online_backup_services

Some examples of online providers are (click on the example to see detailed information):
Dropbox
This is a Web based file hosting service operated by Dropbox, Inc. that uses cloud computing to enable users to store and share files and folders with others across the Internet using file synchronisation. 

There are both free and paid services, each with varying options. Dropbox offers a relatively large number of user clients across a variety of desktop and mobile operating systems.
Google Drive
Google Drive is an online service which provides 15GB of storage for free, allowing files to be accessible from anywhere. A Google account is required to use the Drive service and enables the creation and editing of files directly within the service, providing the means to collaborate and share files with others (including documents, spreadsheets, presentations, forms, and drawings).
Memopal
Memopal is a cloud-based storage application and service that enables users to store and synchronise computer files and share files and folders with others using the Internet.

Source: Wikipedia: http://en.wikipedia.org/wiki/Memopal
FilesAnywhere
FilesAnywhere is one of the first cloud-based storage services to emerge and today continues to offer customers, both consumer and business, a means to back up, edit, sync, collaborate, and share data as well as catalog photos, videos, and music.

Source: Wikipedia: http://en.wikipedia.org/wiki/FilesAnywhere
OneDrive
OneDrive (previously SkyDrive, Windows Live SkyDrive and Windows Live Folders) is a file hosting service that allows users to upload and sync files to a cloud storage and then access them from a Web browser or their local device. It is part of the suite of online services formerly known as Windows Live and allows users to keep the files private, share them with contacts, or make the files public. Publicly shared files do not require a Microsoft account to access.

Source: Wikipedia: http://en.wikipedia.org/wiki/OneDrive
Tresorit
Tresorit is an online cloud storage service based in Switzerland and Hungary that emphasizes enhanced security and data encryption. The service offers users 5 GB of data for free, though it has offered 50 GB to users through promotions with Lifehacker and GigaOM for a limited period of time. It has been likened to a high-security alternative to Dropbox.

Source: Wikipedia: http://en.wikipedia.org/wiki/Tresorit
iCloud
iCloud is a cloud storage and cloud computing service from Apple Inc. launched on October 12, 2011. The service provides its users with means to store data such as documents, photos, and music on remote servers for download to iOS, Macintosh or Windows devices, to share and send data to other users, and to manage their Apple devices if lost or stolen. The service also provides the means to wirelessly back up iOS devices directly to iCloud, instead of being reliant on manual backups to a host Mac or Windows computer using iTunes.

Source: Wikipedia: http://en.wikipedia.org/wiki/ICloud
Advantages
	•	
	•	No user intervention is required (changing tapes, labeling CDs, performing manual tasks)
	•	
	•	Remote backup maintains data off-site
	•	
	•	Most provide versioning and encryption
	•	
	•	They are multi-platform
	•	

Disadvantages
	•	
	•	• Many cloud storage services operate on servers physically located outside the European Economic Area (EEA). It is important that UK users must NEVER use online storage platforms located outside the EEA to store sensitive personally identifiable data, as this is very likely to breach a key principle of the Data Protection Act 1998 – that personal information should not be transferred outside the EEA without adequate protection – which is against UK law.
	•	
	•	Restoration of data may be slow (dependent upon network bandwith)
	•	
	•	Stored data may not be entirely private (if unencrypted)
	•	
	•	Service provider may go out of business
	•	
	•	Protracted intellectual property rights/copyright/data protection licences
	•	
	•	Vendor lock-in, i.e. vendor’s proprietary formats may make migration to another vendor complex and expensive


## Security strategies
Data security means ensuring that research data are kept safe from corruption and that access is suitably controlled.


It is important to consider the security of your data to prevent:
	•	Accidental or malicious damage/modification to data.
	•	
	•	Theft of valuable data.
	•	
	•	Breach of confidentiality agreements and privacy laws.
	•	
	•	Premature release of data, which can void intellectual property claims.
	•	
	•	Release before data have been checked for accuracy and authenticity.

You need to consider the following questions for securing your research data:
	•	How will you manage access arrangements and data security?
	•	
	•	How will you enforce permissions, restrictions and embargoes?
	•	
	•	Other security issues such as sensitive data, off-network storage, storage on mobile devices (laptops, smartphones, flash drives, etc), policy on making copies of data, etc. where relevant.

Securing research data is part of the issue of information technology security. You should always have up to date anti-virus software installed on your office and home computers.

If you have sensitive data that are covered by privacy laws or confidentiality agreements, it is best to store them on a computer that is not connected to any network. If this is not possible, then you can also consider encrypting your data or your PC.

However, you should also be aware of physical security. A computer that is not connected to a network is still vulnerable to theft and malicious damage/modification to data.

Highly sensitive data, regardless of physical storage medium (laptop, USB flash drives, CDs/DVDs), should be stored in a locked room or safe when not in use. Such data should not be stored or transmitted without encryption.
Two issues which are often overlooked but are worth highlighting are 'usernames' and 'passwords' They are so common users often forget they are still a key part of security on most systems.

If possible:
	•	
	•	Never use your username as your e-mail address e.g. fbloggs27@staffmail.ed.ac.uk.
	•	
	•	Instead use an alias e.g.: Fred.Bloggs@ed.ac.uk.
	•	
	•	Do not write passwords on Post-Its or say them aloud as you type.
	•	
	•	Do not log in to secure spaces on untrusted computers or networks (e.g. internet cafés).
	•	
	•	Do not use the obvious (car reg., phone no., pet’s name)
	•	
	•	Do not use any dictionary words (including foreign) on their own.
	•	
	•	Never use the same password for a cloud service, that you use for a University service. For example, to do so is against University of Edinburgh Computer Regulations.
	•	

A guide on creating strong passwords is available on University of Edinburgh Information Services web pages.

What is encryption?

Encryption is the process of converting data into an unreadable code. You must have access to a password or a secret encryption key to be able to read an encrypted file.

Encrypting your data will help ensure your data remain safe from disclosure in the event that a laptop or other portable device such as a USB flash drive/memory stick ends up lost or stolen.

The University of Edinburgh Data Encryption policy warns users that "medium and high risk personal data or business information must be encrypted if it leaves the University environment".

BitLocker (Windows) and FileVault (Mac) are currently the University of Edinburgh's recommended software solution for encrypting data on computers and laptops.

Please note the following considerations before encrypting your data:

Data encryption is not a substitute for other information protection controls.

Data encryption is reliant on the creation of a strong password.

Encrypted data cannot be recovered in the event of a failure.

If the encryption key is lost, the disk image gets corrupted, or the hard disk fails, any encrypted data will be lost.

Establish a reliable and secure backup procedure for the data and any related passwords.


For further information on encryption visit IS/Computing Services pages on encryption:
www.ed.ac.uk/infosec/how-to-protect/encrypting

Encryption of laptops is also an obvious step for laptop security. However, for laptop encryption there is no "one size fits all" solution. Bit Locker, Pretty Good Privacy (PGP) and some other commercial software packages are available, however, you need to consider the operating system.

BitLocker (formerly BitLocker Drive Encryption) is a full disk encryption feature included with the Ultimate and Enterprise editions of Windows Vista and Windows 7, the Pro and Enterprise editions of Windows 8 and Windows 8.1, the Pro, Enterprise, and Education editions of Windows 10, and Windows Server 2008 and later. It is designed to protect data by providing encryption for entire volumes. See Wikipedia for further information: 
http://en.wikipedia.org/wiki/BitLocker

Pretty Good Privacy (PGP) is a data encryption and decryption computer program that provides cryptographic privacy and authentication for data communication. PGP is often used for signing, encrypting, and decrypting texts, e-mails, files, directories, and whole disk partitions and to increase the security of e-mail communications. See Wikipedia for further information:
http://en.wikipedia.org/wiki/PGP_Desktop

If you keep sensitive data on USB flash drives it is recommended that you use drives with encryption software. They give protection to the data if the drive is lost - especially important if the data contain personal or commercially sensitive data. Compared with 'ordinary' USB flash drives they cost only a modest amount more so are a good buy. Your local IT support service will probably be happy to advise on the suitability of any encrypted flash drive that you are planning on purchasing.

You can create a special type of encrypted container in which you can place sensitve data and documents. See this page for more details:
www.ed.ac.uk/infosec/how-to-protect/encrypting/encrypted-containers

Once research on data which includes sensitive data no longer requires that the identifiable portions of the data be retained, they should be destroyed and future research be done with de-identified or anonymised data. This applies to paper records, as well as electronic records.

File deletion is not enough to ensure that sensitive electronic data are completely removed from a computer system. File deletion removes only the pointers to the disk sectors in which the data reside. Deleted files can be recovered using commonly available software tools.

To ensure the complete destruction of sensitive data, the main options are:

•	data erasure (aka data clearing or data wiping) i.e. removing all data while leaving the hard drive or other storage medium still operable - current techniques may not, however, be completely successful on solid-state drives and USB flash drives;

degaussing, which disturbs the magnetic alignment of magnetic storage media and in many cases makes newer media (such as hard drives and tapes) unusable;

physical destruction, through disintegration, shredding, pulverizing or incineration.


More advice on secure deletion when disposing of a device is available here: www.ed.ac.uk/infosec/how-to-protect/secure-deletion



<!-- *Show options from the perspective of a spreadsheet*
### Spreadsheets
- pros/cons from the data management perspective
- Easy to share and to lose track

### Databases
- Easy to share and maintain consistent
- needs a manager -->



## Location and maintenance
Data Backup Options

Hard drive using software like:
Windows 8 File History
OS X Time Machine
Linux/UNIX rsync)
Tape backup system
Many institutions provide a service similar to UCBackup at UC Berkeley. Check with your campus IT support to see if backup service is available. Alternately, your academic department may provide storage space and backup services.
Cloud storage - some examples of private sector storage resources include:
Amazon S3 and Glacier—Requires client software, no encryption support
S3-based Remote Hard Drive Services such as Elephant Drive and Jungle Disk.
Mozy (from EMC) Free client software, 448-bit Blowfish encryption or AES key
Carbonite Free
Test your backup system

To be sure that your backup system is working, periodically retrieve your data files and confirm that you can read them. You should do this when you initially set up the system and on a regular schedule thereafter.

Other data preservation considerations

Who is responsible for managing and controlling the data?

Who controls the data (e.g., the PI, a student, your lab, your university, your funder)? Before you spend a lot of time figuring out how to store the data, to share it, to name it, etc. you should make sure you have the authority to do so.

For what or whom are the data intended?

Who is your intended audience for the data? How do you expect they will use the data? The answer to these questions will help inform structuring and distributing the data.

How long should the data be retained?

Is there any requirement that the data be retained? If so, for how long? 3-5 years, 10-20 years, permanently? Not all data need to be retained, and some data required to be retained need not be retained indefinitely. Have a good understanding of your obligation for the data's retention.

Beyond any externally imposed requirments, think about the long-term usefulness of the data. If the data is from an experiment that you anticipate will be repeatable more quickly, inexpensively, and accurately as technology progresses, you may want to store it for a relatively brief period. If the data consists of observations made outside the laborartory that can never be repeated, you may wish to store it indefinitely.

- From: DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)


Your data are the life blood of your research. If you lose your data, recovery could be slow, costly or worse, it could be impossible. 

Therefore, through the course of your research you must ensure that all your research data, regardless of format, are stored securely, backed up and maintained regularly.

You should estimate the volume of data required for your project at an early stage, probably while drawing up your data management plan. It is also a good idea to consider including costs for data storage in funding proposals.

These may all sound like common sense to you now but the time will come when you will be glad that you have considered these issues right at the beginning of your research and taken the necessary precautions.

You can store your research data on networked drives, personal computers/laptops, and external storage devices. Click on the heading to view detailed information on each option.

Networked drives
Networked drives are managed by staff centrally or within your School or College. It is highly recommended that you store your research data on regularly backed up networked drives such as:
	•	
	•	DataStore, which is storage for active data for all reseach staff and students. It is fully backed-up, secure, resilient, and has multi-site storage. Every researcher is automatically allocated 500 GB storage space for free. Up to 250 GB of each allocation can be shared to create group space. Additional space can be purchased for £200 per TB per year. It is accessible via VPN (Virtual Private Network) from outside the University.
	•	
	•	Fileservers managed by your research group or school.
	•	

This way you will ensure that your data will be:
	•	
	•	Stored in a single place and backed up regularly.
	•	
	•	Available to you as and when required.
	•	
	•	Stored securely minimising the risk of loss, theft or unauthorised use.

Personal computers and laptops


External storage devices
External storage devices such as hard drives, USB flash drives (also known as memory sticks, USB keyrings or pen drives), Compact Discs (CDs) and Digital Video Discs (DVDs), can be an attractive option for storing your data due to their low cost and portability. However, they are not recommended for the long term storage of your data, particularly your master copies, as:
	•	
	•	Their longevity is not guaranteed, especially if they are not stored correctly, for example CDs, DVDs and magnetic tapes degrade over the long term. They can be easily damaged, misplaced or lost.
	•	
	•	Errors writing to CDs and DVDs are fairly common.
	•	
	•	They may not be big enough for all the research data, so multiple disks or drives may be needed.
	•	
	•	They pose a security risk due to their portability.
	•	
If you choose to use CDs, DVDs and USB flash drives (for example, for working data or extra backup copies), you should:

Ensure your master copy is safe and is kept up to date on a networked drive.

Choose high quality products from reputable manufacturers.

Follow the instructions provided by the manufacturer for care and handling, including environmental conditions and labelling.

Regularly check the media to make sure that they are not failing, and periodically 'refresh' the data (that is, copy to a new disk or new USB flash drive).

Ensure that any private or confidential data is encrypted.

What do you think would be the advantages of storing your data on the central, or school networked drives?
If you store your data on the university networked drives your data will be stored in a single place and backed up regularly. The risk of loss, theft or unauthorised use will be minimised as the data will be stored securely on these networked drives. Your data will also be available to you as and when required. Therefore, you should keep at least one copy of your master data files on the networked services.
Keeping backups is probably the most important data management task. There is a real risk of losing data through hard drive failure or accidental deletion. It is therefore recommended that you keep at least 3 copies of your data on at least 2 different media, keeping storage devices in separate locations with at least 1 off-site, and check that they work regularly. You should also have a policy for maintaining regular backups.





- MANTRA "Storage and security" [module](http://mantra.edina.ac.uk/storageandsecurity/)


 Best-practices for storing your file calls for redundancy. Files back up are to have 3 regular back ups of your files. One local ..., one ... and one remote.

 Encryption and Compression

 Unencrypted data will be more easily read by you and others in the future, but you may need to encrypt sensitive data.

 Use mainstream encryption tools (e.g., PGP)
 Don't rely on 3rd party encryption alone
 Keep passwords and keys on paper (2 copies)
 Uncompressed data will be also be easier to read in the future, but you may need to compress files to conserve disk space.

 Use a mainstream compression tool (e.g., ZIP, GZIP, TAR)
 Limit compression to the 3rd backup copy
 Backups and storage

## Security
The security precaustions needed for your data will depend on your project.

As we discussed in the "Legal and ethical considerations" section, ff you're working with ... data, you're responsible for maintaining confidentiality of identifiable data. Make sure to work with your advisor and your research team to  make sure the 

This means data on your computer may need to be kept safe. Or you may be given access to a secure system that stores the data. In which case, you should be careful with your login credentials and be aware of policies moving or sharing the data. 

### Fun fact: Login passwords on your computer are easy to bypass
Your computer password doesn't necessarily keep your data safe. Unless your files are encrypted on your computer, someone who has physical access to your computer can get access to your data with enough effort.

How? Basiclaly, your computer's hard drive can be used like a big USB stick. File permissions for a user are set by your operting system. If someone boots your hard drive with their operating system, those permissions are irrelevant. This can involve different strategies for Macs and PCs, but in both cases it's easy to do with a bit of effort and Googling.

As a precaution, encypt your hard drive.

Find out More: 

PC example: hard drive taken out of computer and mounted on another host gives them access. 
Mac example: Connecting your Mac to another Mac and booting your Mac in Target Disk Mode, your Mac's hard drive will appear as a mounted drive on the other Mac. Unless Mac1 is encrypted with FileVault, all files will be accessible [website](https://support.apple.com/kb/PH10725?locale=en_US)*

## References
- DMPTool. "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)

## Materials
