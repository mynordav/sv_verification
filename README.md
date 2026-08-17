# sv_verification

Hands-on SystemVerilog verification exercises, worked through alongside four books:

1. **SystemVerilog for Verification: A Guide for Learning the Testbench Language Features**, 3rd Edition, Chris Spear & Greg Tumbush — [books/01_systemverilog_for_verification/](books/01_systemverilog_for_verification/)
2. **The UVM Primer: An Introduction to the Universal Verification Methodology**, 1st Edition, Ray Salemi — [books/02_uvm_primer/](books/02_uvm_primer/)
3. **SystemVerilog Assertions Handbook: for Dynamic and Formal Verification**, Revised 4th Edition (2023), Ben Cohen — [books/03_sva_handbook/](books/03_sva_handbook/)
4. **Formal Verification: An Essential Toolkit for VLSI Design**, 2nd Edition, Erik Seligman, Tom Schubert & M. V. Achutha Kiran Kumar — [books/04_formal_verification_toolkit/](books/04_formal_verification_toolkit/)

Each book has one folder per chapter, self-contained (DUT + testbench/properties + run instructions).

## Toolchain

Exercises run on the OSS CAD Suite (Verilator, Yosys, SymbiYosys, GTKWave, cocotb).
Setup notes, installer, and toolchain smoke tests live in `toolchain/` — that
folder is gitignored here since it's local environment setup, not book
exercise content. See `toolchain/tutorials/TOOLCHAIN_TUTORIAL.md` for tool
usage and `toolchain/tutorials/WSL_SETUP.md` for the WSL2 + Ubuntu + VS Code setup.

```bash
source ~/tools/oss-cad-suite/environment
```
