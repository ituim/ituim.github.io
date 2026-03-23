# How to contribute

## Coding conventions

- We indent using three spaces
- ...

## Error handling

- If a routine can fail it shall return a status code.
- Any other value returned from a function shall be used
  only if the status encodes a successful execution.
- Status codes ranges from $\mathtt{0_{16}}$ to $\mathtt{FFFF_{16}}$.
- Status codes from $\mathtt{0_{16}}$ to $\mathtt{3FFF_{16}}$ are reserved
  for the ABI.
  - The value $\mathtt{0_{16}}$ means success.
- Status codes from $\mathtt{4000_{16}}$ to $\mathtt{7FFF_{16}}$ are reserved
  for the OS.
- Status codes from $\mathtt{8000_{16}}$ to $\mathtt{FFFF_{16}}$ are reserved
  for third part libraries.