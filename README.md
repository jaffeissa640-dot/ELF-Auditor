# ELF-Auditor
Security auditing tools for Linux ELF binaries (Version 1 and Version 2)

## License
This software is proprietary. See [LICENSE.txt](LICENSE.txt) for details.  
You may not redistribute, copy, or sell this software without permission.

---

## Version 1 – Compile and Run

1. **Compile**
    gcc elf_auditor_v1.c -o elf-auditor-v1
2. **Run**
    ./elf-auditor-v1 <binary-name>

> Example:
    ./elf-auditor-v1 /bin/ls

---

## Version 2 – Compile and Run

1. **Compile**
    gcc -Wall elf_auditor_v2.c -o elf-auditor
2. **Run**
    ./elf-auditor --help
    ./elf-auditor --scan <binary>
    ./elf-auditor --json <binary>
    ./elf-auditor --risk <binary>
    ./elf-auditor --report <binary>

> Example:
    ./elf-auditor --scan /bin/ls

---

## Directory Structure

    ELF-Auditor/
    ├── LICENSE.txt
    ├── README.md
    ├── src/
    │   ├── elf_auditor_v1.c
        └── elf_auditor_v2.c
    

