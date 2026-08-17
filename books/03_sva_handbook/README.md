# SystemVerilog Assertions Handbook: for Dynamic and Formal Verification

Revised 4th Edition, 2023. Ben Cohen.

Exercises and worked examples from the book, one folder per chapter.
Each chapter folder is self-contained: DUT(s), SVA properties, and a
run script/README (Verilator supports full SVA for simulation-based
checking; SymbiYosys/Yosys only supports immediate assertions + `$past()`
for formal, see [../04_formal_verification_toolkit/](../04_formal_verification_toolkit/)).

## Chapters

- [ch01_intro/](ch01_intro/) — placeholder, add exercises as you read

## Running exercises

Activate the toolchain first (see [../../toolchain/tutorials/TOOLCHAIN_TUTORIAL.md](../../toolchain/tutorials/TOOLCHAIN_TUTORIAL.md)):

```bash
source ~/tools/oss-cad-suite/environment
```
