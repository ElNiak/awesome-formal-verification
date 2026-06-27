<div align="center">
  <a href="https://awesome.re">
    <img src="https://awesome.re/badge-flat2.svg" alt="Awesome">
  </a>
</div>

# Awesome Formal Verification

Welcome to the ultimate list of resources for formal verification/model checking techniques and tools. This repository aims to provide an organized collection of high-quality resources to help professionals, researchers, and enthusiasts stay updated and advance their knowledge in the field.

## Contents

* [Software Verification](#software-verification)
* [Hardware Verification](#hardware-verification)
* [Blogs](#blogs)
* [Conferences](#conferences) 
* [Books](#books)
* [Courses](#courses)
* [More](#more)


## Software Verification

### Tools

#### Formal Verification

* [Panther](https://github.com/ElNiak/PANTHER) - This tool presents a novel approach to bolstering network protocol verification by integrating the Shadow network simulator with the Ivy formal verification tool to check time properties. Furthermore, it extends Ivy's capabilities with a dedicated time module, enabling the verification of complex quantitative-time properties. 
* [ivy](https://github.com/microsoft/ivy) - IVy is a research tool/language intended to allow interactive development of protocols and their proofs of correctness and to provide a platform for developing and experimenting with automated proof techniques.
* [Uppaal](https://uppaal.org/) - Uppaal is an integrated tool environment for modeling, validation and verification of real-time systems modeled as networks of timed automata, extended with data types (bounded integers, arrays, etc.).
* [BLAST](https://cseweb.ucsd.edu/~rjhala/blast.html) - BLAST is a software model checker for C programs. The goal of BLAST is to be able to check that software satisfies behavioral properties of the interfaces it uses. Blast uses counterexample-driven automatic abstraction refinement to construct an abstract model which is model checked for safety properties. The abstraction is constructed /on-the-fly/, and only to the /required precision/. The BLAST project is supported by the National Science Foundation . 
* [PRISM](https://www.prismmodelchecker.org/) -  PRISM is a probabilistic model checker, a tool for formal modelling and analysis of systems that exhibit random or probabilistic behaviour. It has been used to analyse systems from many different application domains, including communication and multimedia protocols, randomised distributed algorithms, security protocols, biological systems and many others.
* [Storm](https://www.stormchecker.org/) Storm is a tool for the analysis of systems involving random or probabilistic phenomena. Given an input model and a quantitative specification, it can determine whether the input model conforms to the specification. Written in C++20, it has been designed with performance and modularity in mind.
* [SPIN](https://spinroot.com/spin/whatispin.html) -  Spin is a widely used open-source software verification tool. The tool can be used for the formal verification of multi-threaded software applications. The tool was developed at Bell Labs in the Unix group of the Computing Sciences Research Center, starting in 1980, and has been available freely since 1991. Spin continues to evolve to keep pace with new developments in the field. In April 2002 the tool was awarded the ACM System Software Award.
* [PLASMA Lab](https://sparika.gitbooks.io/plasma-lab-book/) -  PLASMA Lab is a compact, efficient and flexible platform for statistical model checking of stochastic models. Though in an early stage of development. PLASMA Lab, is being integrated into the DALi and DANSE project platforms.
* [TLA+](https://lamport.azurewebsites.net/tla/tla.html) - TLA+ is a high-level language for modeling programs and systems--especially concurrent and distributed ones.  It's based on the idea that the best way to describe things precisely is with simple mathematics.
* [Quint](https://quint.sh/docs/getting-started) - Quint is a formal specification language where specs are executable: they can be model checked, randomly simulated, and used for edge test case generation and model-based testing against production code. Designed for engineers verifying distributed systems, AI-generated code, and other systems with complex flows. Built on TLA+ semantics with a modern, approachable syntax.
* [Alloy](https://alloytools.org/) - Alloy is a high-level formal modeling language for specifying structural and behavioural aspects of systems using simple mathematics (first-order logic and relations). Comes with a bounded model checker which can find both satisfying and falsifying examples, as well as a unique visualization tool.
* [Rocq](https://rocq-prover.org/) (formerly known as Coq) - Formal proof management system.
* [Isabelle](https://isabelle.in.tum.de/) - Generic proof assistant.
* [HOL](https://hol-theorem-prover.org/) - Proof assistant for higher-order logic.
* [LEAN](https://leanprover.github.io/) - Theorem prover developed at Microsoft Research.
* [ProofOS](https://github.com/Aevion-ai/ProofOS) - Receipt-chained proof obligation ledger for Lean 4. Publishes a machine-readable open-obligation surface (Godel register) with SHA-256 canonical receipts and a multi-agent counsel colony for adversarial review.
* [Verity](https://github.com/th0rgal/verity) - Lean 4 framework for formally specified and verified smart contracts, with EVM-oriented compilation.
* [K Framework](http://www.kframework.org/index.php/Main_Page) - Rewrite-based executable semantic framework.
* [Viper](https://www.pm.inf.ethz.ch/research/viper.html) - Language and tools for permission-based reasoning.
* [Why3](https://www.why3.org/) - Why3 is a platform for deductive program verification. It provides a rich language for specification and programming, called WhyML, and relies on external theorem provers, both automated and interactive, to discharge verification conditions.
* [Frama-C](https://frama-c.com/) - Frama-C is an extensible and collaborative platform dedicated to source-code analysis of C software.


#### Coverage

* [A Practical Approach to Coverage in Model Checking](https://www.cs.huji.ac.il/~ornak/publications/cav01.pdf) - Scientific paper.

#### Linting and Parsing

* [ivy-syntax-highlight](https://github.com/Consensys/ivy-syntax-highlight) - Bare minimum syntax highlight definitions (most likely incomplete) for the Ivy language.

### Languages

* [ivy](https://kenmcmil.github.io/ivy/) - IVy is a research tool/language intended to allow interactive development of protocols and their proofs of correctness and to provide a platform for developing and experimenting with automated proof techniques.
* [Caml](https://caml.inria.fr/) - Caml is a general-purpose programming language, designed with program safety and reliability in mind. It is very expressive, yet easy to learn and use. Caml supports functional, imperative, and object-oriented programming styles. It has been developed and distributed by INRIA, a French research institute in computer science and applied mathematics, since 1985. 

## Hardware Verification

### Tools

#### Formal Verification

* [Symbiyosys](https://symbiyosys.readthedocs.io/en/latest/quickstart.html#prerequisites) - SymbiYosis a front-end driver program for Yosys-based formal hardware verification flows. SymbiYosys provides flows for the following formal tasks: Bounded verification of safety properties (assertions), Unbounded verification of safety properties, Generation of test benches from cover statements, Verification of liveness properties.
* [ABC](https://github.com/berkeley-abc/abc) - ABC: System for Sequential Logic Synthesis and Formal Verification. ABC notably provides combinational equivalence checking (CEC) and sequential equivalence checking (SEQ) engines.
* [riscv-formal](https://github.com/SymbioticEDA/riscv-formal) - A re-usable formal verification framework for RISC-V CPU designs.
* [MCY](https://github.com/YosysHQ/mcy) - MCY is a new tool to help digital designers and project managers understand and improve testbench coverage. Given a self checking testbench, mcy generates 1000s of mutations by modifying individual signals in a post synthesis netlist. These mutations are then filtered using Formal Verification techniques, keeping only those that can cause an important change in the design's output. All mutated designs are run against the testbench to check that the testbench will detect and fail for a relevant mutation. The testbench can then be improved to get 100% complete coverage.
* [EBMC / CBMC](http://www.cprover.org/ebmc/) - EBMC is a Model Checker for hardware designs. It includes both bounded and unbounded analysis, i.e., it can both discover bugs and is also able to prove the absence of bugs. It can read Netlists (ISCAS89 format), Verilog, System Verilog and SMV files. Properties can be given in LTL or a fragment of System Verilog Assertions.
* [seL4](https://sel4.systems/) - Operating-system kernel with an end-to-end proof of implementation correctness and security enforcement.
  * [brochure](https://sel4.systems/Info/Docs/seL4-brochure.pdf)
  * [white paper](https://sel4.systems/Info/Docs/GD-NICTA-whitepaper.pdf)
* [Certikos](http://flint.cs.yale.edu/certikos/) - Certified Kit Operating System. Formally verified compiler for C.
* [Compcert](http://compcert.inria.fr/) 
  * [C compiler](http://compcert.inria.fr/download.html)
* [Bedrock](http://plv.csail.mit.edu/bedrock/) - Rocq (previously Coq) library for verification.
  * [tutorial pdf](http://plv.csail.mit.edu/bedrock/tutorial.pdf)
* [HACMS](https://www.darpa.mil/program/high-assurance-cyber-military-systems) - High-Assurance Cyber Military Systems.
  * [more Darpa "formal" tagged links](https://www.darpa.mil/tag-list?tt=78)
* [Genode](http://genode.org/) - Novel OS architecture.

  
#### Simulation

* [Verilator](https://www.veripool.org/projects/verilator/wiki/Intro) - Verilator is  "the fastest free Verilog HDL simulator". From a verification perspective it supports *line coverage*, *signal toggle coverage* and limited specification of *functional coverage* using SystemVerilog Assertions. It also allows one to write testbenches in C++ or SystemC.
* [Icarus Verilog](https://github.com/steveicarus/iverilog) - The excellent Icarus Verilog simulator. Slower than Verilator, but it supports full 4-state simulation (i.e. X's and Z's).

#### Build Systems and Continuous Integration

* [LibreCores CI](https://www.librecores.org/static/librecores-ci) - LibreCores CI is a service, which provides Continuous Integration of projects being hosted on LibreCores. The objective of the service is to improve the contributor experience and to increase trust to projects by providing automated testing and health metrics of the projects.
* [FuseSoc](https://github.com/olofk/fusesoc) - FuseSoC is an award-winning package manager and a set of build tools for HDL (Hardware Description Language) code. Its main purpose is to increase reuse of IP (Intellectual Property) cores and be an aid for creating, building and simulating SoC solutions.

#### Test / Program / Code Generators

* [AAPG (Automated Assembly Program Generator)](https://gitlab.com/shaktiproject/tools/aapg) - Generator for assembly programs.
* [riscv-dv](https://github.com/chipsalliance/riscv-dv) - Instruction sequence generator for RISC-V.
* [rggen](https://github.com/rggen/rggen) - Code generation tool for configuration and status registers.
* [FORCE-RISCV](https://github.com/openhwgroup/force-riscv) - Instruction sequence generator for RISC-V.

#### Coverage

* [covered](https://github.com/anders-code/verilog-covered) - Coverage analysis tool.

#### Linting and Parsing

* [svlint](https://github.com/dalance/svlint) - Linter for SystemVerilog.
* [sv-parser](https://github.com/dalance/sv-parser) - SystemVerilog parser.
* [Surelog](https://github.com/chipsalliance/Surelog) - SystemVerilog pre-processor and parser.

#### Testbench Frameworks

* [cocotb](https://www.cocotb.org/) - Python based testbench environment for many simulators.
* [cocotb-coverage](https://cocotb-coverage.readthedocs.io) - Functional coverage and constrained randomization extensions for Cocotb.
* [fvutils/pyvsc](https://github.com/fvutils/pyvsc) - Python packages providing a library for verification stimulus and coverage.
* [chiselverify](https://github.com/chiselverify/chiselverify) - UVM-like verification for the Chisel HDL.
* [UVVM](https://github.com/UVVM/UVVM) - Universal VHDL Verification Methodology.
* [OSVVM](https://osvvm.org/) - Open Source VHDL Verification Methodology.
* [VUnit](https://vunit.github.io/) - Unit testing framework for VHDL/SystemVerilog.
* [V3](https://pmc.ncbi.nlm.nih.gov/articles/PMC9806438/) - Verification framework.
* [ROHD Verification Framework](https://github.com/intel/rohd-vf) - Hardware verification framework upon ROHD for building and executing testbenches.

#### Components / VIPs

* [uvm_axi](https://github.com/funningboy/uvm_axi) - AXI bus verification IP.
* [AXI Bus Formal VIP](https://github.com/kumarrishav14/AXI) - Formal verification IP for AXI bus.
* [AXI Bus Functional Model tvip-axi](https://github.com/taichi-ishitani/tvip-axi) - Functional model for AXI bus.
* [AXI SystemVerilog Modules and Verification Infrastructure](https://github.com/pulp-platform/axi) - SystemVerilog modules and verification infrastructure for AXI bus.
* [APB Bus Functional Model tvip-apb](https://github.com/taichi-ishitani/tvip-apb) - Functional model for APB bus.
* [USB 1.1 Test Suite](https://github.com/antmicro/usb-test-suite-testbenches) - Test suite for USB 1.1.
* [Cocotb Verification IPs](https://github.com/themperek/cocotb-vivado) - Various cocotb packages for common interfaces: AXI/Ethernet/PCIE.
* [RISC-V-TLM](https://github.com/mariusmm/RISC-V-TLM) - A SystemC transaction level model of RISC-V.

### Languages

* [Idris](https://www.idris-lang.org/) - General purpose pure functional programming language with dependent types.
  * [Idris docs](http://docs.idris-lang.org/en/latest/)
  * [Idris tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)
  * [Theorem proving with Idris tutorial](http://docs.idris-lang.org/en/latest/proofs/index.html)
* [Agda](http://wiki.portal.chalmers.se/agda/pmwiki.php) - Dependently typed functional programming language.
  * [Agda GitHub](https://github.com/agda/agda)
  * [Agda User Manual](http://agda.readthedocs.io/en/v2.5.2/)
* [UR/Web](http://www.impredicative.com/ur/) - Ur plus a special standard library for dynamic web applications.
* [Haskell](https://www.haskell.org/) - An advanced, purely functional programming language.
* [Liquid Haskell](https://ucsd-progsys.github.io/liquidhaskell-blog/) - Refines Haskell's types with logical predicates for compile-time property enforcement.
* [Elm](http://elm-lang.org/) - Type-safe functional programming language for declaratively creating web browser-based graphical user interfaces.


## Blogs

* [Dan Gisselquist Formal Verification Blogs](https://zipcpu.com/formal/formal.html) - Blog posts on formal verification.
* [Verification Gentleman Blog](https://blog.verificationgentleman.com/) - Blog on verification topics.
* [Bits, Bytes and Gates](https://bitsbytesgates.com/) - Blog covering formal verification and hardware design.

## Conferences

* [ORCONF](https://orconf.org) - Open Source Digital Design Conference.
* [OSDA](https://www.offsec.com/courses/soc-200/) - Open Source Digital Architecture workshop.
* [CHIPS Alliance Workshop on Open Source Design Verification](https://www.chipsalliance.org) - Workshop on open source design verification.
* [Workshop on Open-Source EDA Technology (WOSET)](https://woset-workshop.github.io) - Workshop on open-source EDA technology.

## Books

* [The Little Prover](https://mitpress.mit.edu/books/little-prover) - Introduction to inductive proofs for computer programs.
* [Certified Programming with Dependent Types](http://adam.chlipala.net/cpdt/) - Textbook on practical engineering with Rocq (previously Coq).
  * [Latest draft](http://adam.chlipala.net/cpdt/cpdt.pdf)
* [Software Foundations](https://softwarefoundations.cis.upenn.edu/) - Introduction to the mathematical underpinnings of reliable software.
  * [Vol. 1: Logical Foundations](https://softwarefoundations.cis.upenn.edu/lf-current/index.html)
  * [Vol. 2: Programming Language Foundations](https://softwarefoundations.cis.upenn.edu/plf-current/index.html)
  * [Vol. 3: Verified Functional Algorithms](https://softwarefoundations.cis.upenn.edu/vfa-current/index.html)
* [HoTT: Homotopy Type Theory: Univalent Foundations of Mathematics](https://homotopytypetheory.org/book/)
  * [pdf](http://saunders.phil.cmu.edu/book/hott-online.pdf)
* [MCB: Mathematical Components](https://math-comp.github.io/mcb/)

## Courses

* [DeepSpec Summer School](https://www.youtube.com/channel/UC5yB0ZRgc4A99ttkwer-dDw) - Videos about deep specification, Rocq (previously Coq) tutorials.
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

