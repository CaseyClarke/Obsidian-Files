
stack
|
\\/
/\
|
heap: dynamic data
static data: global vairables
text: code
reserved

caller saved registers: ra, t_, a_, 
callee saved registers sp, fp, s_

freq = cycles / second
clock cycle = seconds / cycles
cpu time = num of cycles / freq
cpi = cycles per instruction
clock cycles = instructions x cpi
cpu time =  instruction count  * clock cycles/ instruction (cpi) * seconds /clock cycle (1/ freq) (clock cycle)

IEEE 754 (sign bit)  (8 exp bits) (23 mantissa bits)
IEEE 754 double (sign bit)  (11 exp bits) (52 mantissa bits)

normalized = 1.(.....) x 2^(....)
0.1111111...
0.5 + 0.25 + 0.125 + ....
infinity = exp all 1's mantissa all 0
NAN = exp all 1's mantissa \neq 0

G = first bit after mantissa
R = second bit after mantiss
S = 1 if any bit after R is 1
GRS
0xx - round down = do nothing
100 - tie, round up if last bit is 1 else round down = do nothing
101,110,111 - round up

bias = 2^(e-1) -1
normalized values have implicit 1

![[Pasted image 20251216185129.png]]


control hazard - This hazard occurs when an instruction depends on the decision of a previous decision-making instruction

data hazard - This hazard occurs when an instruction needs data from a previous instruction in order to execute correctly

Structural Hazard - This hazard occurs when a resource is busy causing an instruction to delay its execution

branch target buffer

When the Hazard detection unit determines that a data dependence cannot be satisfied by forwarding, it must make the instruction function as a no-op. To do so, it sets all the control signals for that instruction to zero. It also forces the instruction fetch stage to repeat the fetching of the same instruction again.

when exception, PC is stored in UPEC

IF ID EX MEM WB

load-use hazard, 
lw then immediately value used, -> need 1 bubble/stall
ID/EX  EX/MEM MEM/WB

block size = words per block * bytes per word
offsetbits = log(block size (bytes))

num blocks = cache size / block size

number of sets = num blocks / associativity

address bits = Tag | Index | offset

1 tag per block

Write allocate: On a write miss, first copy the data into the local cache, then perform the write on the cached copy.

Write back: Writes update only the local cached copy; changes are written back to the repository later (e.g., when finished or evicted).

Write through: Every write to the local copy is immediately written to the repository as well.

Write around: On a write miss, write directly to the repository without creating or updating a local cached copy.

N = total number of instructions
FLS​ = fraction of load/store instructions
MRI= instruction cache miss rate
MRD = data cache miss rate
HRD=1−MRD
MP = miss penalty (cycles)
HT = hit time (cycles)
CPIdeal = CPI with perfect cache

I-Cache accesses = N
D-Cache access = N * FLS

I cache misses = N * MRI
D-cache misses = N * FLS * MRD
TOTAL memory requests N * MRI + N * FLS * MRD

MR_AVG = MRI + FLS * MRD

AMAT = HT + MR_AVG * MP

total accesses = N+N * FLS