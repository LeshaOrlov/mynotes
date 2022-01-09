# Install
Created вторник 09 Ноябрь 2021

**error: linker `link.exe` not found**

**Case 1:** Using C++ win compiler, to fix it you need to reinstall VS build tool C++ Download the Visual Studio 2019 Build tools from the Microsoft website: <https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16>

After the download, while installing the Build tools, make sure that you install the required components:

C++ build tools

This will download required files. Once everything is successfully installed, reboot and re-run your rust program and it will compile successfully.

**Case2:** This error can come from the fact that you use GCC to compile, to fix it (assume that you already have MinGW):

Tape in cmd:

rustup uninstall toolchain stable-x86_64-pc-windows-msvc
rustup toolchain install stable-x86_64-pc-windows-gnu (or download rustup-init for the platform of your choice at <https://forge.rust-lang.org/infra/other-installation-methods.html>)
rustup default stable-x86_64-pc-windows-gnu

**Case 3:** You don't want to download Visual studio with build tools, simply install MinGw with g++ gcc development packages, then run CASE 2

