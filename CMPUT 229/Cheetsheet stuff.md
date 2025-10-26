risc-v word is 32 bits / 4 bytes
risv-v is little endian i.e lowest signifigance bytes stored in lowest memory address
slii t2, s0, k = t2 <- s0 x 2^k
slii / slri max 31 bits "operand out of range error" otherwise
sll /slr exists
srai / slai sign extends instead of just 0
cant do "and rd, rs1, 0xsomething" as it tries to exend the hex to 32 bits which is too large for instruction