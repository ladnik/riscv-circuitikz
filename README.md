# riscv-circuitikz (A RISC-V Processor Components CircuiTikZ Library)
This CircuiTikZ library offers some components to efficiently draw RISC-V processors in LaTeX. The library was designed with the goal of resembling the RISC-V processor schematics as presented in "Digital Design and Computer Architecture: RISC-V Edition" by Sarah L. Harris and David Harris.
For more information, refer to the documentation in this repository.

## Usage
Documentation can be found at [`doc/manual.pdf`](/doc/manual.pdf), the library file itself in [`lib/`](/lib). This library is based on TikZ and CircuiTikZ, so make sure these packages are properly installed and included in your document preamble (refer to section 1.2 of the documentation).

## Examples
Below are some example figures created using components from this library. Both of them and further figures can be found at [`doc/figures/`](/doc/figures/).

![Single-Cycle RISC-V Processor](/doc/images/riscv_sc.png)

![Pipelined RISC-V Processor](/doc/images/riscv_pl.png)

If you have any questions regarding this project or ideas on improving it, feel free to open an issue or a pull request.
