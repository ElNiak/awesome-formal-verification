# Awesome Formal Verification

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

Welcome to the ultimate list of resources for formal verification techniques and tools. This repository aims to provide an organized collection of high-quality resources to help professionals, researchers, and enthusiasts stay updated and advance their knowledge in the field.

Inspired by [awesome-provable](https://github.com/awesomo4000/awesome-provable) and [awesome-open-hardware-verification](https://github.com/ben-marshall/awesome-open-hardware-verification)!

## Table of Contents

* [Tools](#tools) which contain or implement verification related functionality
* [Languages](#languages) - Languages with good ability to use formal type safety
* [Proof Assistants](#proof-assistants) - Interactive theorem provers used to prove properties of programs.
* [Projects](#projects) - Projects involving provably correct code.
* [Books](#books) - Textbooks commonly referred to
* [Courses](#courses) - Online courses (YouTube, university courses)
* [Testbench Frameworks](#frameworks) which make writing testbenches easier
* [Verification Guides](#guides) and blog posts on how to actually go about verifying a hardware design
* [Conferences](#conferences) where new work on open source hardware verification is talked about
* [More Links](#more) - Video presentations about formal proof of code topics

## Tools

### Formal Verification

- [Symbiyosys](#symbiyosys) - Tool suite for formal verification of RTL designs.
- [riscv-formal](#riscv-formal) - RISC-V formal verification framework.
- [MCY](#mcy) - Testbench coverage tool.
- [EBMC / CBMC](#ebmc--cbmc) - Model checker for C/C++ and hardware designs.

### Simulation

- [Verilator](#verilator) - Verilog Simulator.
- [Icarus Verilog](#icarus-verilog) - Icarus Verilog Simulator.

### Build Systems and Continuous Integration

- [LibreCores CI](#librecores-ci) - Continuous integration service for open hardware.
- [FuseSoc](#fusesoc) - Package manager and build abstraction tool for FPGA/ASIC development.
  - [fsva](#fsva) - FuseSoC Verification Automation.

### Test / Program / Code Generators

- [AAPG (Automated Assembly Program Generator)](#aapg) - Generator for assembly programs.
- [riscv-dv](#riscv-dv) - Instruction sequence generator for RISC-V.
- [rggen](#rggen) - Code generation tool for configuration and status registers.
- [FORCE-RISCV](#force-riscv) - Instruction sequence generator for RISC-V.

### Coverage

- [covered](#covered) - Coverage analysis tool.

### Linting and Parsing

- [svlint](#svlint) - Linter for SystemVerilog.
- [sv-parser](#sv-parser) - SystemVerilog parser.
- [Surelog](#surelog-system-verilog-2017-pre-processor-parser) - SystemVerilog pre-processor and parser.

## Testbench Frameworks

- [cocotb](#cocotb) - Python based testbench environment for many simulators.
  - [python-uvm](#python-uvm) - A port of UVM 1.2 to Python and cocotb.
  - [cocotb-coverage](#cocotb-coverage) - Functional coverage and constrained randomization extensions for Cocotb.
  - [Verification IPs](#cocotb-ips) - Various cocotb packages for common interfaces: AXI/Ethernet/PCIE.
- [fvutils/pyvsc](#fvutilspyvsc) - Python packages providing a library for verification stimulus and coverage.
- [chiselverify](#chisel-verify) - UVM-like verification for the Chisel HDL.
- [UVVM](#uvvm) - Universal VHDL Verification Methodology.
- [OSVVM](#osvvm) - Open Source VHDL Verification Methodology.
- [VUnit](#vunit) - Unit testing framework for VHDL/SystemVerilog.
- [V3](#v3) - Verification framework.
- [ROHD Verification Framework](#rohd-verification-framework) - Hardware verification framework upon ROHD for building and executing testbenches.

## Components / VIPs

- [uvm_axi](#uvm_axi) - AXI bus verification IP.
- [AXI Bus Formal VIP](#axi-bus-formal-vip) - Formal verification IP for AXI bus.
- [AXI Bus Functional Model tvip-axi](#axi-bus-functional-model---tvip-axi) - Functional model for AXI bus.
- [AXI SystemVerilog Modules and Verification Infrastructure](#axi-systemverilog-modules-and-verification-infrastructure) - SystemVerilog modules and verification infrastructure for AXI bus.
- [APB Bus Functional Model tvip-apb](#apb-bus-functional-model---tvip-apb) - Functional model for APB bus.
- [USB 1.1 Test Suite](#antmicro-usb-test-suite) - Test suite for USB 1.1.
- [Cocotb Verification IPs](#cocotb-ips) - Various cocotb packages for common interfaces: AXI/Ethernet/PCIE.
- [RISC-V-TLM](#risc-v-tlm) - A SystemC transaction level model of RISC-V.

## Guides & Blogs

- [Dan Gisselquist Formal Verification Blogs](#dan-gisselquist-formal-verification-blogs) - Blog posts on formal verification.
- [Verification Gentleman Blog](#verification-gentleman-blog) - Blog on verification topics.
- [Bits, Bytes and Gates](#bits-bytes-and-gates) - Blog covering formal verification and hardware design.

## Conferences

- [ORCONF](#orconf) - Open Source Digital Design Conference.
- [OSDA](#osda) - Open Source Digital Architecture workshop.
- [CHIPS Alliance Workshop on Open Source Design Verification](#chips-alliance-workshop-on-open-source-design-verification) - Workshop on open source design verification.
- [Workshop on Open-Source EDA Technology (WOSET)](#workshop-on-open-source-eda-technology-woset) - Workshop on open-source EDA technology.

## Languages

* [Idris](https://www.idris-lang.org/) - General purpose pure functional programming language with dependent types.
  * [Idris docs](http://docs.idris-lang.org/en/latest/)
  * [Idris tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)
  * [Theorem proving with Idris tutorial](http://docs.idris-lang.org/en/latest/proofs/index.html)
* [Agda](http://wiki.portal.chalmers.se/agda/pmwiki.php) - Dependently typed functional programming language.
  * [Agda Github](https://github.com/agda/agda)
  * [Agda User Manual](http://agda.readthedocs.io/en/v2.5.2/)
* [UR/Web](http://www.impredicative.com/ur/) - Ur plus a special standard library for dynamic web applications.
* [Haskell](https://www.haskell.org/) - An advanced, purely functional programming language.
* [Liquid Haskell](https://ucsd-progsys.github.io/liquidhaskell-blog/) - Refines Haskell's types with logical predicates for compile-time property enforcement.
* [Elm](http://elm-lang.org/) - Type-safe functional programming language for declaratively creating web browser-based graphical user interfaces.
* [ivy](https://kenmcmil.github.io/ivy/) - IVy is a research tool/language intended to allow interactive development of protocols and their proofs of correctness and to provide a platform for developing and experimenting with automated proof techniques.

  
## Proof Assistants

* [Coq](https://coq.inria.fr/) - Formal proof management system.
  * https://github.com/Ptival/PeaCoq
  * https://math-comp.github.io/mcb/
* [Isabelle](https://isabelle.in.tum.de/) - Generic proof assistant.
  * [overview](https://isabelle.in.tum.de/overview.html)
* [HOL](https://hol-theorem-prover.org/) - Proof assistant for higher-order logic.
  * [Other HOLS](https://hol-theorem-prover.org/other-hols.html)
* [LEAN](https://leanprover.github.io/) - Theorem prover developed at Microsoft Research.
  * [Online version](https://leanprover.github.io/live/latest/)
* [K Framework](http://www.kframework.org/index.php/Main_Page) - Rewrite-based executable semantic framework.
  * [K Tutorial](http://www.kframework.org/index.php/K_Tutorial) by [Grigore Rosu](https://github.com/grosu), [video playlist](https://www.youtube.com/watch?v=eSaIKHQOo4c&list=PLx_U8qR-tMtLQEDPvVk1y9gTIdUIWGaQd)
* [Viper](https://www.pm.inf.ethz.ch/research/viper.html) - Language and tools for permission-based reasoning.

## Projects

* [seL4](https://sel4.systems/) - Operating-system kernel with an end-to-end proof of implementation correctness and security enforcement.
  * [brochure](https://sel4.systems/Info/Docs/seL4-brochure.pdf)
  * [white paper](https://sel4.systems/Info/Docs/GD-NICTA-whitepaper.pdf)
* [Certikos](http://flint.cs.yale.edu/certikos/) - Certified Kit Operating System.
  * [Certified OS Kernels](http://flint.cs.yale.edu/certikos/)
* [Compcert](http://compcert.inria.fr/) - Formally verified compiler for C.
  * [C compiler](http://compcert.inria.fr/download.html)
* [Bedrock](http://plv.csail.mit.edu/bedrock/) - Coq library for verification.
  * [tutorial pdf](http://plv.csail.mit.edu/bedrock/tutorial.pdf)
* [HACMS](https://www.darpa.mil/program/high-assurance-cyber-military-systems) - High-Assurance Cyber Military Systems.
  * [more Darpa "formal" tagged links](https://www.darpa.mil/tag-list?tt=78)
* [Genode](http://genode.org/) - Novel OS architecture.

## Books

* [The Little Prover](https://mitpress.mit.edu/books/little-prover) - Introduction to inductive proofs for computer programs.
* [Certified Programming with Dependent Types](http://adam.chlipala.net/cpdt/) - Textbook on practical engineering with Coq.
  * [Latest draft](http://adam.chlipala.net/cpdt/cpdt.pdf)
* [Software Foundations](https://softwarefoundations.cis.upenn.edu/) - Introduction to the mathematical underpinnings of reliable software.
  * [Vol. 1: Logical Foundations](https://softwarefoundations.cis.upenn.edu/lf-current/index.html)
    * [read](https://softwarefoundations.cis.upenn.edu/lf-current/toc.html)
    * [download](https://softwarefoundations.cis.upenn.edu/lf-current/lf.tgz)
  * [Vol. 2: Programming Language Foundations](https://softwarefoundations.cis.upenn.edu/plf-current/index.html)
    * [read](https://softwarefoundations.cis.upenn.edu/plf-current/toc.html)
    * [download](https://softwarefoundations.cis.upenn.edu/plf-current/plf.tgz)
  * [Vol. 3: Verified Functional Algorithms](https://softwarefoundations.cis.upenn.edu/vfa-current/index.html)
    * [read](https://softwarefoundations.cis.upenn.edu/vfa-current/index.html)
    * [download](https://softwarefoundations.cis.upenn.edu/vfa-current/vfa.tgz)
* [HoTT: Homotopy Type Theory: Univalent Foundations of Mathematics](https://homotopytypetheory.org/book/)
  * [pdf](http://saunders.phil.cmu.edu/book/hott-online.pdf)
* [MCB: Mathematical Components](https://math-comp.github.io/mcb/)

## Courses

* [DeepSpec Summer School](https://www.youtube.com/channel/UC5yB0ZRgc4A99ttkwer-dDw) - Videos about deep specification, Coq tutorials.
* Adam Chlipala Videos:
  * [Coming Soon Machine-Checked Mathematical Proofs in Everyday Software and Hardware Development](https://media.ccc.de/v/34c3-9105-coming_soon_machine-checked_mathematical_proofs_in_everyday_software_and_hardware_development)
  * [Lecture 1, OPLSS 2015](https://www.youtube.com/watch?v=ORKAy_CHDYM)
  * [Bedrock: A Software Development Ecosystem Inside a Proof Assistant](https://www.youtube.com/watch?v=BSyrp-iYBMo)
  * [Ur/Web: A Simple Model for Programming the Web](https://www.youtube.com/watch?v=J3XI6-aZZXk)
  * [Proof Engineering](https://www.youtube.com/watch?v=yXLeyANzAC4)
  * [Coq Proof Assistant and Its Applications to Programming-Language Semantics](https://www.youtube.com/playlist?list=PLt7hcIEdZLAnO7AawDQkHwE7RtwPDOFEc)
* [Type-Drive Development in Idris - Edwin Brady](https://www.youtube.com/watch?v=X36ye-1x_HQ)
* [Benjamin Pierce - Software Foundations Course](https://www.youtube.com/playlist?list=PLGCr8P_YncjUT7gXUVJWSoefQ40gTOz89)
* [Learning Automated Theorem Proving](https://cs.stackexchange.com/questions/820/learning-automated-theorem-proving) - Stackexchange post about learning.

## More

* [Curry-Howard](https://en.wikipedia.org/wiki/Curry%E2%80%93Howard_correspondence) - Direct relationship between computer programs and mathematical proofs.
* [Hoare logic](https://en.wikipedia.org/wiki/Hoare_logic) - Formal system for reasoning rigorously about the correctness of computer programs.
* [Designing A Theorem Prover (Paulson, Cambridge, 1990)](https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-192.pdf)
* [Rolf Rolles Program Synthesis in Reverse Engineering](https://www.youtube.com/watch?v=mFjSbxV_1vw) - Assume you generate all possible programs.
* [The Open-Source seL4 Kernel. Military-Grade Security Through Mathematics - SFO17-417](https://www.youtube.com/watch?v=heSmrHzHcuM)
* [DARPA Hack Proof Drones](https://www.defensetech.org/2014/05/21/darpa-unveils-hack-proof-drone/)
* [Pentagon Wants Unhackable Helicopters](https://www.engadget.com/2015/03/16/pentagon-wants-unhackable-helicopters/)
* [Hacker-Proof Code Confirmed](https://www.quantamagazine.org/formal-verification-creates-hacker-proof-code-20160920/) - Computer scientists can prove certain programs to be error-free with the same certainty that mathematicians prove theorems.
* [CertiKOS enables creation of secure system kernels](http://www.zdnet.com/article/certikos-a-hacker-proof-os/) - Secure concurrent kernel for x86 and ARM.
* [seL4 Is Free – What Does This Mean For You?](https://www.youtube.com/watch?v=lRndE7rSXiI)
* [From L3 to seL4: What Have We Learnt in 20 Years of L4 Microkernels?](https://www.youtube.com/watch?v=RdoaFc5-1Rk)
* [seL4 introduction: Capability--based Access Model](https://www.youtube.com/watch?v=x3P6Y6VO0UI) - Chinese, translation?
* [seL4 playlist](https://www.youtube.com/playlist?list=PL8UO9ZG39Nx43YCAKGCtj9Rb6p2_3utdc)
* [Creating drones that can't be hacked](https://www.youtube.com/watch?v=4oONdV5RYp8)
* [HACMS: Protecting Military Systems from Hackers](https://www.youtube.com/watch?v=OyqNpn6JpBk)

## Contributing

Your contributions are always welcome! Feel free to submit a pull request with your suggestions.
