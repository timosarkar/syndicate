# syndicate
heavy-armored, stealth LD_PRELOAD rootkit

## Features

- Exploitation of LD_PRELOAD in order to inject itself into all running processes
- Loads a virtual filesystem where all system-required data are loaded into. The virtual filesystem can be hidden by LD_PRELOAD abuse in order to create a two-layer security mechanism
- Every trace on the network is obfuscated and hidden by injecting custom BPF bytecode into each packet. This allows syndicate to be hidden from sniffing tools such as nmap and wireshark.
- Anti-Emulation routine
- Anti-Forensics by dropping files into a loaded vfs which itself is hidden by LD_PRELOAD
- Encrypted telegram backdoor
