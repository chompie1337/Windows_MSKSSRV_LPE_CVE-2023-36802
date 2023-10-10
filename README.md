# CVE-2023-36802 Local Privilege Escalation POC

authors: [chompie](https://twitter.com/chompie1337)

For demonstration purposes only. Complete exploit works on vulnerable Windows 11 22H2 systems. 
Adapting the exploit to all vulnerable systems is left as an exercise to the reader. Git gud, etc. 

Usage:

```
Windows_MSKSSRV_LPE_CVE-2023-6802.exe <pid>
```

where `<pid>` is the process ID (in decimal) of the process to elevate.

Should result in the target process being elevated to SYSTEM


The I/O Ring LPE primitive code is based on the I/ORing R/W [PoC](https://github.com/yardenshafir/IoRingReadWritePrimitive) by [Yarden Shafir](https://twitter.com/yarden_shafir)

Blog post [here](https://securityintelligence.com/posts/critically-close-to-zero-day-exploiting-microsoft-kernel-streaming-service/)