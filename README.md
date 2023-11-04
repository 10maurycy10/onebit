# Designs:

## CPU

- \[DONE\] \[TESTED\] Instruction decoder 
- \[DONE\] \[TESTED\] Register
- \[DONE\] \[FIXED\] \[TESTED\] ALU control logic
- \[DONE\] \[FIXED\] \[TESTED\] Logic unit
- \[DONE\] Adder
- \[DONE\] Bus driver
- Skip logic
- Clock generator
- Write control/OEN logic

## ROM

- Program counter
- ROM board (softwere!)

## MEMORY

- Offset handling
- Row addressing
- Bit addressing
- Bit array/maped io

## Front panel

Functions:
Inspect memory 16 bits at a time
View ACC/Carry, HLT
Start, Stop, Single Step

- Panel
- Pulse generator for start

# CPU BOM:

- `instruction_decoder/decoder_not` * 4 (1/each opcode bit)
- `instruction_decoder/decoder_nor` * 16 (1/each instruction)
- `register` * 7 (2 ACC, 2 Carry, 1 OEN, 2 Skip) 
- `alu_control` * 1
- `alu` * 1
- `adder` * 1
- `bus_driver` * 1
