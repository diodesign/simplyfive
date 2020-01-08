# simplyfive

This is a simple 32-bit [RISC-V](https://riscv.org/specifications/) soft processor core implementation, specifically RV32I, in Verilog using [nMigen](https://github.com/m-labs/nmigen). This is my first attempt at developing a modern CPU: please don't expect it to be perfect. It's a personal learning experience.

I hope to one day get it up to RV32G compatibility, or at least RV32IMAC so it can boot a proper operating system.

## Todo

This is a work in progress. Here's what needs to be implemented:
* Instruction fetch
* Instruction decode
* Instruction execution:
  * lui
  * auipc
  * jal
  * jalr
  * beq
  * bne
  * blt
  * bge
  * bltu
  * bgeu
  * lb
  * lh
  * lw
  * lbu
  * lhu
  * sb
  * sh
  * sw
  * addi
  * slti
  * sltiu
  * xori
  * ori
  * andi
  * slli
  * srli
  * srai
  * add
  * sub
  * sll
  * slt
  * sltu
  * xor
  * srl
  * sra
  * or
  * and
  * More to add to this list...
* Memory and register writeback
* Register file
* CSRs
* Exceptions and interrupts
* PMP and MMU
* Supervisor and User modes
* M, A, C extensions
* Branch prediction
* Instruction and data cache

## Copyright, license, and contact

Copyright &copy; Chris Williams, 2020. See [LICENSE](https://github.com/diodesign/simplyfive/blob/master/LICENSE) for distribution and use of source code and binaries.

Please [email](mailto:diodesign@tuta.io) me if you have any questions or issues to raise, wish to get involved, have source to contribute, or have found a security flaw. You can, of course, submit pull requests or raise issues via GitHub, though please consider disclosing security-related matters privately. Please include `simplyfive` in the subject line if you do email in any case.
