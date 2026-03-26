# ELF-Auditor
Security auditing tools for Linux ELF binaries (Version 1 and Version 2).
ELF-Auditor helps you quickly assess ELF binaries for security risks, identify risky functions, and generate professional reports.
1. **Version 1 (Community Edition)** – Free, open-source, basic scanning features.
2. **Version 2 (Professional Edition)** – Paid version, with additional professional features unlocked via a license key.


## License
This software is proprietary. See [LICENSE.txt](LICENSE.txt) for details.  
You may not redistribute, copy, or sell this software without permission.

---

## Version 1 – Usage:(Community Edition)
1. Unzip the file
    unzip elf-auditor_v1.zip
2. Make it executable
    chmod +x elf-auditor-v1
3. Basic scan
    ./elf-auditor-v1 /path/to/binary

> Example:
    ./elf-auditor-v1 /bin/ls
### Features:
- Detect **PIE** (Position Independent Executable)
- Detect **NX** (Non-Executable Stack)
- Detect **RELRO** (Read-Only Relocations)
- Lightweight and fast, suitable for quick scans
- Single command usage

## Version 1 Example Output:
```
PIE: ENABLED
NX: ENABLED                                                                                                                                                                                                                               
RELRO: PRESENT                                                                                                                                                                                                                          
Stack Canary: PRESENT                                                                                                                                                                                                 
Potentially Risky Functions Detected:
  strcpy
  memcpy
```
---

## Version 2 – Usage:(Professional Edition)

1. Unzip the file
    unzip version2-auditor.zip
2. Make it executable
    chmod +x version2-auditor
3. Basic scan
    ./Version2 --help
    ./Version2 --scan path/to//binary
    ./Version2 --json /path/to/binary
    ./Version2 --risk /path/to/binary
    ./Version2 --report /path/to/binary
## Version 2 Example Output: 
./Version2 --scan path/to/binary
```
NX: ENABLED
PIE: ENABLED
RELRO: FULL
Stack Canary: PRESENT
RPATH: None

Potentially Risky Functions Detected:
    X : FUNC    GLOBAL DEFAULT  UND strcpy@GLIBC_X.X.X 
    X : FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_X.X 

Potentially Risky Functions Detected:
    X : FUNC    GLOBAL DEFAULT  UND strcpy@GLIBC_X.X.X 
    X : FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_X.X 
Stack Canary: PRESENT
RPATH: None

Risk Score: 0 (LOW)
Contributing Factors:
  Stack Canary: PRESENT (+0)
  NX: ENABLED (+0)
  PIE: ENABLED (+0)
  RELRO: FULL (+0)
  Risky Functions Detected:
    X : FUNC    GLOBAL DEFAULT  UND strcpy@GLIBC_X.X.X 
    X : FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_X.X 

```


## Directory Structure

    ELF-Auditor/
    ├── LICENSE.txt
    ├── README.md
    ├── src/
        ├── elf_auditor_v1.zip
        
    

