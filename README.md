I like to make computer go beep boop
```asm
.global _start
.intel_syntax noprefix

_start:
        mov rax, 1
        mov rdi, 1
        mov rdx, 61
        lea rsi, [message]
        syscall

        mov rax, 60
        mov rdi, 0
        syscall

message:
        .byte 0x52,0x6F,0x73,0x65,0x73,0x20,0x61,0x72,0x65,0x20,0x72,0x65,0x64,0x0A
        .byte 0x56,0x69,0x6F,0x6C,0x65,0x74,0x73,0x20,0x61,0x72,0x65,0x20,0x62,0x6C,0x75,0x65,0x0A
        .byte 0x49,0x20,0x68,0x61,0x74,0x65,0x20,0x53,0x63,0x72,0x75,0x6D,0x0A
        .byte 0x41,0x6E,0x64,0x20,0x62,0x75,0x72,0x6E,0x6F,0x75,0x74,0x20,0x74,0x6F,0x6F,0x0A,0x00
```
