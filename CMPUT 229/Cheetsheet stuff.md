risc-v word is 32 bits / 4 bytes
risv-v is little endian i.e lowest signifigance bytes stored in lowest memory address
slii t2, s0, k = t2 <- s0 x 2^k
slii / slri max 31 bits "operand out of range error" otherwise
sll /slr exists
srai / slai sign extends instead of just 0
cant do "and rd, rs1, 0xsomething" as it tries to exend the hex to 32 bits which is too large for instruction

stack
|
\\/
/\
|
heap: dynamic data
staic data: global vairables
text: code
reserved

caller saved registers: ra, t_, a_, 
callee saved registers sp, fp, s_

relative perf
$\frac{perf_a}{perf_b} = \frac{time_b}{time_a} = n$
freq = cycles / second
clock cycle = seconds / cycles
clock cycle = 1/ freq
cpu time = num of cycles / freq
cpi = cycles per instruction
clock cycles = instructions x cpi

summary 

cpu time =  instruction count  * clock cycles/ instruction (cpi) * seconds /clock cycle (1/ freq) (clock cycle)

power is proportional to 1/2 capacitive load * voltage^2 * frequency

amdahls law -> improving one aspect of a computer doesn't mean the computer has that proportional improvment

x = \*p
if registers lw a1, 0(a0)
if memory
lw s1, -4(s0)
lw s1, 0(s1)
sw s2, -12(s0)

ucause stores the reason for exception
most sig bit is 0 if exception 1 if interupt

ustatus least sig bit is 0 if user interupts disabled 1 if enabled

interupt enable register (uie) example 4th bit is enable external timer interrupt 8th is enable external keyboard interupt

atomic read write csr

csrr2 t0, 0, t1
t0 <- CSR0 (zero extended)
CSR0 <- t1

csrrwi t0, 0, immediate

csrrc t0, 0, t1
basically anywhere where the bit of t1 = 1 that bit is cleared in CSR0

csrrci t0, 0, immediate
if immediate is 0 just copy csr0 into t0

csrrs t0, 0, t1 
anywhere t1 is 1 set that bit in CSR0

csrrsi t0, 0, immidiate
t0 = csr0
csr0 = csr0 or immidiate


|   |   |   |
|---|---|---|
|**CSRRW rd, csr, rs1**|_Atomic Read/Write_|`t = CSR[csr]; CSR[csr] = x[rs1]; x[rd] = t` — reads the CSR into `rd` and writes the value from `rs1` to it.|

|   |   |   |
|---|---|---|
|**CSRRS rd, csr, rs1**|_Atomic Read and Set Bits_|`t = CSR[csr]; CSR[csr] = t OR x[rs1]; x[rd] = t` — sets bits in the CSR that are 1 in `rs1`.|

|                        |                              |                                                                                                   |
| ---------------------- | ---------------------------- | ------------------------------------------------------------------------------------------------- |
| **CSRRC rd, csr, rs1** | _Atomic Read and Clear Bits_ | `t = CSR[csr]; CSR[csr] = t AND ~x[rs1]; x[rd] = t` — clears bits in the CSR that are 1 in `rs1`. |

![[Pasted image 20251026183219.png]]

privilege 

0 user
1 supervisor
2 reserved
3 machine

trap level, vertical trap, increase priviliege
horizontal, don't

![[Pasted image 20251026183434.png]]

![[Pasted image 20251026183451.png]]

write allocate write through write around ...

critical selection = thing you are accessing
race condition
starvation 
deadlock