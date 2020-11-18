# ARM CMake Project Generator

## Usage
```
ARM CMake project generator

Usage: arm-create-project [options] project-name
Options:
  -c, --compiler <value>      Compiler for the project, options are: 'gcc', 'clang' or 'all' (default is 'gcc')
  -d, --destination <value>   Destination path of the project without project-name (default is current directory)
  -q, --quiet                 Quiet mode
  --gcc-bin <value>           Path of GCC bin directory
  --clang-bin <value>         Path of Clang/LLVM bin directory
  --libgcc <value>            Path of libgcc base (required by Clang, defaults to trying to find it)
  -h, --help                  Display this help and exit

Exit status:
  0 if OK
  1 if error
```

## Info
* Clang/LLVM for ARM cortex still somewhat uses GCC (libgcc), at least in this configuration.
* This setup has been tested on Linux only.
* Currently, everything is configured for a "generic" ARM cortex-m4 **without** an FPU (can be changed in config-m4).
* This is as bare-metal as you can get, it will probably not directly work on any real-world ARM cotrex-m? mcu.

