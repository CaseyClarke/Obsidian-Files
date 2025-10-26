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
callee saved registers sp, s_

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
