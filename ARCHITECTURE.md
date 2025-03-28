# Callstack Spoofing Library Architecture

## Core Components
- `SpoofFunc`: XOR-encrypts return addresses
- `SpoofCall`: Template-based function wrapper
- Shellcode generator: Copies functions to executable memory

## Key Features
- Dual-mode support (User/Kernel)
- Dynamic function size detection
- Memory safety mechanisms
- Cross-platform compatibility

## Usage
```cpp
SPOOF_FUNC; // Spoof current function
auto result = SPOOF_CALL(int, foo)(args...);
```