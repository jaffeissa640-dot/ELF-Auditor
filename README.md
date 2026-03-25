# ELF-Auditor
Security auditing tools for Linux ELF binaries (Version 1 and Version 2)
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
3. First Run
    ./elf-auditor-v1 /path/to/binary

> Example:
    ./elf-auditor-v1 /bin/ls

---

## Version 2 – Usage:(Professional Edition)

1. Unzip the file
    unzip version2-auditor.zip
2. Make it executable
    chmod +x version2-auditor
3. First Run
    ./Version2 --help
    ./Version2 --scan path/to//binary
    ./Version2 --json /path/to/binary
    ./Version2 --risk /path/to/binary
    ./Version2 --report /path/to/binary

## Directory Structure

    ELF-Auditor/
    ├── LICENSE.txt
    ├── README.md
    ├── src/
        ├── elf_auditor_v1.zip
        
    

