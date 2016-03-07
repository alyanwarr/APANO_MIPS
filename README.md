# APANO MIPS
## MIPS Datapath And Control Unit Simulator (Assembly)
 Project APANO MIPS aims to implement a low-level MIPS datapath and control unit
simulator. Datapath simulation includes simulating all its components (registers, memories,
ALUs, multiplexers, shifters, sign extenders , and the connections among these). User is able
to input a program (using the supported instructions) to be simulated, as well as specifying it's
starting address. APANO MIPS keeps track of the register file contents and memory contents.

APANO MIPS supports the following instructions:
* Arithmetic: add, addi, sub
* Load/Store: lw, sw
* Logic: sll, and, or, nor
* Control flow: beq, bne, j, jal, jr
* Comparison: slt, slti,sltu,sltui

## Installation
`git clone https://github.com/alyanwarr/APANO_MIPS.git`

## Usage
Program starts with a message box informing user with instructions supported, and step-by-
step guide on how to use the program including the correct format to enter his/her
instructions.

<img src="https://cloud.githubusercontent.com/assets/12968456/13578974/ac555552-e4a3-11e5-8265-d1c0f7c551a8.png" width="400">

User is then redirected into a window where he/she should write his/her MIPS instructions ,
then press "RUN" to submit the instructions entered.

<img src="https://cloud.githubusercontent.com/assets/12968456/13579155/89ac7ed0-e4a4-11e5-81b6-3a00b18ef859.png" width="400">

Simulation process starts when user presses "RUN" button.

<img src="https://cloud.githubusercontent.com/assets/12968456/13579156/89ca7534-e4a4-11e5-9989-89ea0080058f.png" width="800">

User shall press "Continue" to keep track of the data path cycle of the current instruction, or
press "NEXT" to go to the second instruction. User can also press the button at any of the data
items to view/keep track of values (reg file, data memory ,) data items.

<img src="https://cloud.githubusercontent.com/assets/12968456/13579154/898194ae-e4a4-11e5-9fee-9fd018bf5ae5.png" widht="800">

## Control Unit Truth Table

<img src="https://cloud.githubusercontent.com/assets/12968456/13579158/89ea6330-e4a4-11e5-9bc4-5ed001734892.png" width="800">
## Contribute

1. Fork it
2. Create your feature branch: `git checkout -b new-feature`
3. Commit your changes: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin new-feature`
5. Submit Pull request

## Credits

#### APANO Team:
* Aly Anwar 
* AbdelRahman Gaafar
* Nour ELDin
* Omar Adel
* Peter Magdi

## License
The MIT License (MIT)

Copyright (c) 2016 Aly Anwar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
