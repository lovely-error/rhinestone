## Things to explore

* Approach execution model from the modern perspective:
    * convinience of ISA for a programmer is not a priority
    * instruction dependencies will be explicitly specified(shallow dependency tagging via biniary sequence breaks)
* Variable length instruction encoding
* Several encoding schemes for instructions
* Register spectrum (used for compact common instructions)
```
[r0][r1][r2][r3][r4][r5][r6][r7]
 ^   ^   ^   ^
  register ground
<- hotter ------------ colder ->
```
* Explicit shallow dependency information encoded into instructions via binary sequence breaks
* Reconfigurable ALU for better simultaneous execution. Units can be configured to execute any opearion of logic or arithmetic
* Not all instructions have 3 operand format. Some use one of select registers to serve both as source and destination
* A way to explicitly specify synchronisation regions per core groups

## Instruction representation
Each instructinon can be of lenth 8, 16 or 32 bits.
Different encoding for different classes of instructions.