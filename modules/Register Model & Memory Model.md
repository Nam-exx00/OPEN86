# OPEN86 Register Model & Memory Model

## Contents

1. Register Model
2. Memory Model

## Register Model

### Contents

1. No Extension

### No Extension

| Name | Count | Description |
|---|---|---|
| General-purpose registers | 8 | `EAX`, `ECX`, `EDX`, `EBX`, `ESP`, `EBP`, `ESI`, `EDI`; also usable as 16-bit or 8-bit registers |
| Instruction pointer | 1 | `EIP`, points to the next instruction to execute |
| Flags register | 1 | `EFLAGS`, holds arithmetic and control flags |
| Segment registers | 6 | `CS`, `DS`, `ES`, `SS`, `FS`, `GS`, for segmented-model compatibility; used as flat memory in no-extension mode |

## Memory Model

### Contents

1. No Extension

### No Extension

No extension is generally **unprotected flat memory**, with a minimum requirement of **1MB**. At startup, the program is usually **loaded at 0x00007C00**.