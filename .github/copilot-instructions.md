# sv_verification repo instructions

Personal SystemVerilog verification learning project (WSL2 + Ubuntu + VS Code),
working through 4 books using the open-source OSS CAD Suite toolchain.

## Toolchain / environment

- Activate before running any tool: `source ~/tools/oss-cad-suite/environment`
  (adds `verilator`, `yosys`, `sby`, `gtkwave` to `PATH`).
- Tools: **Verilator** (simulation, `--binary --trace`), **Yosys** (synthesis
  sanity checks), **SymbiYosys**/`sby` (formal: BMC/prove/cover — note Yosys's
  Verilog frontend only supports immediate assertions + `$past()`, not full
  SVA `property`/`|=>` syntax, for formal proofs), **GTKWave** (waveform
  viewing), **cocotb** (Python testbenches — bundled with the suite's own
  Python interpreter `tabbypy3`; never `pip install cocotb` separately or mix
  with system Python).
- Details/examples: [toolchain/tutorials/TOOLCHAIN_TUTORIAL.md](toolchain/tutorials/TOOLCHAIN_TUTORIAL.md)
  and [toolchain/tutorials/WSL_SETUP.md](toolchain/tutorials/WSL_SETUP.md).

## Repo layout

- `books/` — git-tracked learning content, one folder per book, one
  subfolder per chapter. See `books/*/README.md` for book titles/editions.
- `toolchain/` — gitignored, local-only: the original installation smoke test
  and environment tutorials. Not part of the book exercises.

## Learning-mode code policy

This is a learning project — see
[.github/instructions/book-exercises.instructions.md](.github/instructions/book-exercises.instructions.md)
for rules on not writing exercise/project code inside `books/**` on the
user's behalf. Code outside `books/**` (toolchain scripts, run scripts,
collateral) has no such restriction.
