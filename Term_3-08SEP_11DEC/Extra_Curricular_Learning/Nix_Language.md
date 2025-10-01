# Nix Language notes

## Basic Syntax
1. Derivations
```nix
derivation{
    name = "program-name';
    system = "aarch64-darwin";
    build = "/usr/bin/clang";
    src = ./main.c;
}
```
The derivation function executes a command and captures the output
system must be specified to avoid conflicts and the builder is the language that's used to compile the code
- Nix is independant from system libraries like C, C++ if Clang is used
