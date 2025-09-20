# RISC-V Reference SoC Tapeout Program VSD

### **System Requirement Check**
- 16 GB RAM
- 100.3 GB SSD available
- OS : Ubuntu 24.04.3 LTS
- Processor : 13th Gen Intel® Core™ i5-1335U × 12

<img width="788" height="697" alt="Screenshot from 2025-09-20 16-32-29" src="https://github.com/user-attachments/assets/a73ae1eb-8bc2-4e96-9b2f-162f9217fc7c" />

### **Tool Check**
#### <ins>**Yosys**</ins>

```bash
$ sudo apt-get update
$ git clone --recurse-submodules https://github.com/YosysHQ/yosys.git
$ cd yosys
$ sudo apt install make               # If make is not installed
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-clang
$ make config-gcc

$ make
$ sudo make install

$ make test

$ yosys
```

<img width="837" height="233" alt="Screenshot from 2025-09-20 16-26-34" src="https://github.com/user-attachments/assets/5bc4885c-15f7-4a95-a6d4-5ec267311bae" />

#### <ins>**Iverilog**</ins>
```bash
$ sudo apt-get update
$ sudo apt-get install iverilog
$ iverlog -v
```

<img width="801" height="676" alt="Screenshot from 2025-09-20 14-00-01" src="https://github.com/user-attachments/assets/3f097ae6-2063-4f39-9b89-e6769aeca9c8" />

#### <ins>**gtkwave**</ins>
```bash
$ sudo apt-get update
$ sudo apt install gtkwave
$ gtkwave -v
```
<img width="787" height="83" alt="Screenshot from 2025-09-20 14-00-15" src="https://github.com/user-attachments/assets/2b7d610f-a428-415d-bdf5-b6ef8ce905bb" />
