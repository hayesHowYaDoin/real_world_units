# Real-World Units Library

This repository is intended to be used for expressing domains which involve
mathematical equations which model the real world. The units in this library
were intended as a way for me to gain practice with the C++ standard library
functions used for building sum types (namely, std::variant and std::visit). 
The overall project layout is inspired by the Boost project 
(https://github.com/boostorg/boost), and uses a Docker Dev Container with 
VSCode.

## Prerequisites

The following instructions assume that Docker, VSCode and Git are installed on 
the host computer. The VSCode extension Remote Development 
(ms-vscode-remote.vscode-remote-extensionpack) is required to open the project 
in a Dev Container. 

## Setting Up The Development Environment

1) Clone the repository onto the host computer with the following command:
   ```
    git clone https://github.com/hayesHowYaDoin/cpp_header_template.git
   ```
2) Open the folder in VSCode. In the Command Palette (Ctrl+Shift+P), execute 
the command "Dev Containers: Open Folder In Container..."

And... that's it!
