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

<img src="https://cloud.githubusercontent.com/assets/12968456/13579155/89ac7ed0-e4a4-11e5-81b6-3a00b18ef859.png" width="350">

Simulation process starts when user presses "RUN" button.

<img src="https://cloud.githubusercontent.com/assets/12968456/13579156/89ca7534-e4a4-11e5-9989-89ea0080058f.png" width="700">

User shall press "Continue" to keep track of the data path cycle of the current instruction, or
press "NEXT" to go to the second instruction. User can also press the button at any of the data
items to view/keep track of values (reg file, data memory ,) data items.

<img src="https://cloud.githubusercontent.com/assets/12968456/13579154/898194ae-e4a4-11e5-9fee-9fd018bf5ae5.png" widht="800">

## Control Unit Truth Table

<img src="https://cloud.githubusercontent.com/assets/12968456/13579158/89ea6330-e4a4-11e5-9bc4-5ed001734892.png" width="800">

## Examples

* Sum all numbers between a user-input defined number and another user-input defined
number.


Code Tested:


`add $t0,$t0,$a0`

`LOOP: slt $t2,$t0,$a1`

`beq $t2,$zero,EXIT`

`add $s0,$s0,$t0`

`addi $t0,$t0,1`

`j LOOP`

`EXIT: add $s0,$s0,$t0`

Data associated : $a0 = 1 , $a1= 10 -> $s0 (at the end) = 55

* Greatest Common Divisor (GCD)

Code Tested:

`gcd: beq $a0,$a1,exit`

`slt $t0,$a1,$a0`

`bne $t0,$zero,L1`

`sub $a1,$a1,$a0`

`j gcd`

`L1: sub $a0,$a0,$a1`

`j gcd`

`exit: add $v0,$a0,$zero`

Data associated: $a0=5 ,$a1 = 15 -> $v0 (at the end) = 5

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
APANO MIPS is licensed under the MIT license. take a look at the [LICENSE](https://github.com/alyanwarr/APANO_MIPS/blob/master/LICENSE) for more information.

