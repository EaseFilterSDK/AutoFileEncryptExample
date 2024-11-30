# [Transparent File Encryption SDK](https://www.easefilter.com/Forums_Files/Transparent_Encryption_Filter_Driver.htm)
 A C# transparent file encryption example was implemented with the Transparent File Encryption Filter Driver SDK. The transparent file encryption performs real-time I/O encryption and decryption of the files in any block data with 16 bytes. The encryption uses a 256 bits symmetric key to encrypt or decrypt the data with AES encryption algorithm. Auto file encryption protects data "at rest", meaning the transparent data and files encryption. It provides the ability to comply with policies which can be applied by users, processes and file type. This allows only authorized users and processes to access the encrypted files, unauthorized users and processes can’t access the encrypted files.
 
![File Encryption](https://www.easefilter.com/Images/TransparentFileEncryption.png)

## The advantages of the EaseFilter Encryption SDK:
1. **Completely transparent file encryption in file system level.** The encryption process was done in the write IO request, the decryption process was done in the read IO request, there are no extra IO request needed, it is completely transparent to the applications or users, the encryption or decryption doesn't require the application to interfere. 
2. **Keep encrypted file on disk all the time.** Since the decryption data only was kept in memory, there are no extra file created for the decryption.
3. **Authorized specific processes or users to read the encrypted file.** EaseFilter Encryption SDK was implemented with Isolation Mini Filter Driver. When the process or the user was authorized to access the encrypted file, the filter driver will decrypt the data in memory during the read request, so the authorized process can get the clear data back, or it will get the raw encrypted data. When the encryption filter driver is turned off, the application will always get the encrypted raw data.
4. **Random block level decryption.** You can decrypt the blocks of the file, you don't need to decrypt the whole file for all the time. For large encrypted file, if you only want to read the blocks of the data, it will improve the performance dramatically.
5. **High encryption or decryption performance.** EaseFilter Encryption Engine utilizes the US FIPS 140-2 compliant Microsoft CNG libraries, it can support AES-NI (or the Intel Advanced Encryption Standard New Instructions; AES-NI), at an algorithm level AES-NI provides significant speedup of AES. For non-Parallel modes of AES operation (CBC encrypt), AES-NI can provide 2-3 fold gain in performance over a completely software encryption. For parallel modes of AES operation (CBC-decrypt, CTR), AES-NI can provide 10x improvement over a completely software encryption.
   

## The products you can develop with EaseFilter Encryption SDK:

1. **Data encryption at rest.** Encryption at rest prevents the attacker from accessing the unencrypted data by ensuring the data is encrypted when on disk.
Data protection.

2. **Document encryption.** File encryption is very important step for data protection, only the authorized users or processes can read the encrypted data, or will get the raw encrypted data.

3. **Data loss prevention.** To prevent the data breach, your data is encrypted all the time, even your data was lost and found in an unauthorized place, they are protected against the unauthorized access.

4. **Secure file sharing with DRM.**
Encrypted your files with digital rights management data embedded into the encrypted header, protect, track and control your encrypted files anywhere anytime, you can grant or revoke the access control to any user at any time even the files were shared.

## A C# Auto File Encryption Example
With the C# auto file encryption example, you can setup an encryption folder in computer A, configure the authorized processes, users who can read the encrypted file, then you can setup the decryption folder in computer B, you can copy the encrypted file to this folder, and configure the authorized processes which can read the encrypted files in the decryption folder.

![File Encryption Demo](https://www.easefilter.com/images/autoencryptdemo.png)

[Read more about auto file encryption example](https://www.easefilter.com/Forums_Files/AutoFileEncryption.htm)


## EaseFilter File System Filter Driver SDK Reference
| Product Name | Description |
| --- | --- |
| [File Monitor SDK](https://www.easefilter.com/kb/file-monitor-filter-driver-sdk.htm) | EaseFilter File Monitor Filter Driver SDK Introduction. |
| [File Control SDK](https://www.easefilter.com/kb/file-control-file-security-sdk.htm) | EaseFilter File Control Filter Driver SDK Introduction. |
| [File Encryption SDK](https://www.easefilter.com/kb/transparent-file-encryption-filter-driver-sdk.htm) | EaseFilter Transparent File Encryption Filter Driver SDK Introduction. |
| [Registry Filter SDK](https://www.easefilter.com/kb/registry-filter-drive-sdk.htm) | EaseFilter Registry Filter Driver SDK Introduction. |
| [Process Filter SDK](https://www.easefilter.com/kb/process-filter-driver-sdk.htm) | EaseFilter Process Filter Driver SDK Introduction. |
| [Storage Tiering SDK](https://www.easefilter.com/cloud/storage-tiering-sdk.htm) | EaseFilter Storage Tiering Filter Driver SDK Introduction. |
| [EaseFilter SDK Programming](https://www.easefilter.com/kb/programming.htm) | EaseFilter Filter Driver SDK Programming. |

## EaseFilter SDK Sample Projects
| Sample Project | Description |
| --- | --- |
| [Auto File DRM Encryption](https://www.easefilter.com/kb/auto-file-drm-encryption-tool.htm) | Auto file encryption with DRM data embedded. |
| [Transparent File Encrypt](https://www.easefilter.com/kb/AutoFileEncryption.htm) | Transparent on access file encryption. |
| [Secure File Sharing with DRM](https://www.easefilter.com/kb/DRM_Secure_File_Sharing.htm) | Secure encrypted file sharing with digital rights management. |
| [File Monitor Example](https://www.easefilter.com/kb/file-monitor-demo.htm) | Monitor file system I/O in real time, tracking file changes. |
| [File Protector Example](https://www.easefilter.com/kb/file-protector-demo.htm) | Prevent sensitive files from being accessed by unauthorized users or processes. |
| [FolderLocker Example](https://www.easefilter.com/kb/FolderLocker.htm) | Lock file automatically in a FolderLocker. |
| [Process Monitor](https://www.easefilter.com/kb/Process-Monitor.htm) | Monitor the process creation and termination, block unauthorized process running. |
| [Registry Monitor](https://www.easefilter.com/kb/RegMon.htm) | Monitor the Registry activities, block the modification of the Registry keys. |
| [Secure Sandbox Example](https://www.easefilter.com/kb/Secure-Sandbox.htm) |A secure sandbox example, block the processes accessing the files out of the box. |
| [FileSystemWatcher Example](https://www.easefilter.com/kb/FileSystemWatcher.htm) | File system watcher, logging the file I/O events. |

## Filter Driver Reference

* Understand MiniFilter Driver: https://www.easefilter.com/kb/understand-minifilter.htm
* Understand File I/O: https://www.easefilter.com/kb/File_IO.htm
* Understand I/O Request Packets(IRPs):https://www.easefilter.com/kb/understand-irps.htm
* Filter Driver Developer Guide: https://www.easefilter.com/kb/DeveloperGuide.htm
* MiniFilter Filter Driver Framework: https://www.easefilter.com/kb/minifilter-framework.htm
* Isolation Filter Driver: https://www.easefilter.com/kb/Isolation_Filter_Driver.htm

## Support
If you have questions or need help, please contact support@easefilter.com 

[Home](https://www.easefilter.com/) | [Solution](https://www.easefilter.com/solutions.htm) | [Download](https://www.easefilter.com/download.htm) | [Demos](https://www.easefilter.com/online-fileio-test.aspx) | [Blog](https://blog.easefilter.com/) | [Programming](https://www.easefilter.com/kb/programming.htm)
