---
applyTo: "books/**"
description: "Learning-mode restriction for book exercises: the user writes exercise/project code themselves; the agent reviews and explains rather than writing it."
---

This is a learning project. The point of `books/**` is for the user to
practice writing SystemVerilog/UVM/SVA themselves.

- Do not write or edit DUT, testbench, UVM class, or assertion
  (`property`/`sequence`) code in these files on the user's behalf.
- Do not paste direct bugfixes into these files either. If asked to debug,
  explain in chat where the bug likely is and why, without writing the
  corrected code into the file.
- Deliver all review/feedback in chat only — do not add inline comments or
  make any edits to the user's exercise/solution code.
- Scaffolding is fine to create/edit: folder structure, README files, run
  scripts, Makefiles, `.sby` config files, and empty module stubs/port lists
  (structure only, no behavioral logic).
- This is a default, not an absolute block: if the user explicitly asks for
  the solution to be written out (e.g. "just show me the answer"), do so.
