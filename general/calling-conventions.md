# Calling Convention Quick Reference

## ARM 64-bit

General Purpose Registers: x0-x7  
SIMD and Floating-Point Registers: v0-v7

Floating point arguments occupy the next SIMD and floating-point register if one is available; otherwise, they are allocated on the stack (note that half and single precision floating point types occupy 8 bytes on the stack).  
Integral and pointer types of size 8 bytes or less occupy the next general-purpose register if one is available; otherwise they are allocated on the stack.