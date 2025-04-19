# DLL-Injector – Educational DLL Injection Tool

## 🔍 Overview

This project demonstrates manual DLL injection by modifying the structure of a Windows Portable Executable (PE) file. The tool appends a new section to the target executable and embeds a specified DLL, simulating low-level techniques used in red teaming and malware analysis.

> **⚠️ Educational Use Only:**  
> This tool is intended solely for educational and research purposes. Do not use it on systems or files you do not own or have explicit permission to test. The author is not responsible for any misuse.

---

## 💡 Features

- Parses and modifies PE file headers using Windows API and raw memory access.
- Injects a DLL into a newly created section in the target executable.
- Aligns section headers correctly in both memory and on disk.
- Low-level Windows programming using `CreateFileA`, `ReadFile`, `WriteFile`, `SetFilePointer`, etc.
- Demonstrates core concepts in reverse engineering, red-team tooling, and PE format internals.

---

## 🛠️ Usage

```bash
EthicalInjector.exe <section_name> <target_exe_path> <dll_path>
