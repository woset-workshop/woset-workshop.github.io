#  WOSET 2021 Proceedings

To cite an article, please use this format:
(author names here), "(article title here)", Article No. (article number here), Workshop on Open-Source EDA Technology (WOSET), 2021.

For live discussions via Zoom and Slack, please see the [WOSET 2021 Schedule](WOSET2021-schedule.md).

## Organization

### Co-Chairs
* Jose Renau, UC Santa Cruz (Co-Chair)
* Matthew Guthaus, UC Santa Cruz (Co-Chair)

### Program Committee
* Matthew Guthaus, UC Santa Cruz
* Jack Koenig, SiFive
* Rajit Manohar, Yale University
* Priyanka Raina, Stanford
* Jose Renau, UC Santa Cruz
* Matthew Venn, Zero to ASIC Course
* Bruno Schmidt, EPFL
* Scott Temple, University of Utah

### Web Chair
* Jesse Cirimeli-Low, UC Santa Cruz

### Virtual Arrangements
* Sakshi Garg, UC Santa Cruz

## Best contribution

Winner
* TBD

Honorable mentions:
* TBD


## Best video

Winner
* TBD

Honorable mentions:
* TBD

# Article 1

## CFU Playground: Build your own ML Processor using Open Source
[paper](PDFs/2021/a01.pdf)
[presentation](Videos/2021/a01-video.mp4)
[slides](PDFs/2021/a01-slides.pdf)
[repo](https://github.com/google/CFU-Playground)

### Abstract
The CFU (Custom Function Unit) Playground allows you to design and build machine learning (ML) accelerators extending an FPGA-based RISC-V core, running on an FPGA board at your desk.
Because the CPU is soft, it can be both tailored (e.g. cache sizes modified) and extended (new instructions added through the use of a Custom Function Unit). Push-button builds of the customized processor combined with a provided interactive software test/measurement harness allows for very rapid edit-compile-profile cycles (on the order of minutes) at each stage of accelerator development.

A primary goal of the CFU Playground is to provide a delightful  and fun experience to the  developer,  by, as far as possible, removing the burden of maintaining infrastructure such as configuring toolchains, writing test harnesses, building performance  measurement jigs, or editing Makefiles.
This rapid, lightweight framework lets the user realize a large performance benefit from a relatively small investment in creating customized hardware.

CFU Playground bundles together open source software (TensorFlow, GCC),  open-source RTL generation IP and toolkits (LiteX, VexRiscv, Migen, nMigen),  and open-source FPGA tools for synthesis, place, and route (yosys, nextpnr, vpr, etc.). By using open source for the entire stack,
% software {\em and} gateware IP,  we give the user access to customize and co-optimize hardware and software, resulting in a specialized solution unencumbered by licensing restrictions
and not tied to a particular FPGA or board.

CFU Playground is available under an Apache 2.0 license at  https://github.com/google/CFU-Playground.   Online documentation is available at https://cfu-playground.readthedocs.io.
### Authors
1. Tim Callahan <tcal@google.com> (Google)
2. Tim Ansell <tansell@google.com> (Google)
3. Joseph Bushagour (Purdue University)
4. Alan V. Green <avg@google.com> (Google)
5. David Lattimore <dml@google.com> (Google)
6. Dan Callaghan <dcallagh@google.com> (Google)

# Article 2

## The Open-Source Bluespec bsc Compiler and Reusable Example Designs

[paper](PDFs/2021/a02.pdf)
[presentation](Videos/2021/a02-video.mp4)
[slides](PDFs/2021/a02-slides.pdf)
[repo](https://github.com/CTSRD-CHERI/bluecheck)

### Abstract

The _bsc_ compiler, which has been in commercial use for two decades, was released as a free and open-source artefact in January 2020. Here we describe briefly _bsc_ and its flows, available tutorial materials, and several reusable open-source designs using _bsc_, many of them centered on RISC-V (from embedded to Linux-capable CPUs and systems), all FPGA-ready.

### Authors
1. Julie Schwartz <quark@bluespec.com> (Bluespec, Inc.)
2. Niraj N. Sharma <niraj.sharma@bluespec.com> (Bluespec, Inc.)
3. Darius Rad <darius@bluespec.com> (Bluespec, Inc.)
4. Ken Takusagawa <ken@bluespec.com> (Bluespec, Inc.)
5. Joe Stoy <stoy@bluespec.com> (Bluespec, Inc.)
6. Rishiyur Nikhil <nikhil@bluespec.com> (Bluespec, Inc.)

# Article 3

## Open-Source Formal Verification for Chisel

[paper](PDFs/2021/a03.pdf)
[presentation](Videos/2021/a03-video.mp4)
[slides](PDFs/2021/a03-slides.pdf)
[repo](https://github.com/ekiwi/open-source-formal-verification-for-chisel)

### Abstract

Chisel is a Scala embedded hardware construction language allowing designers to take advantage of a general purpose programming language to generate digital circuit descriptions. From the beginning Chisel has featured integration with RTL simulators in order to allow designers to unit test their designs. We recently added support for easy formal verification of Chisel designs. Our implementation will be available to all users of the next Chisel and chiseltest releases. The source code is hosted on github and published under a permissive Apache 2 license.

### Authors
1. Kevin Laeufer <laeufer@berkeley.edu> (University of California, Berkeley)
2. Jonathan Bachrach <jrb@berkeley.edu> (University of California, Berkeley)
3. Koushik Sen <ksen@berkeley.edu> (University of California, Berkeley)

# Article 4

## Automating GDS Generation in Magic

[paper](PDFs/2021/a04.pdf)
[presentation](Videos/2021/a04-video.mp4)
[slides](PDFs/2021/a04-slides.pdf)
[repo](http://www.opencircuitdesign.com/magic)

## Abstract

The Magic layout editor has always been outside of the mainstream in EDA tools in its concept that custom manual layout should be simple and straightforward while remaining essentially unconstrained.  Magic does this by hiding various implant layers, marker layers, and cut layers from the designer.  As a consequence, it has to generate all these layers automatically during GDS format mask data generation.  This is an extremely difficult problem.  I will present a variety of examples requiring sophisticated decision-making on automated layout, strategies for producing DRC-correct layout, and a discussion of recent enhancements to Magic's GDS-generation engine and what further development work is required

### Author

tim@opencircuitdesign.com

# Article 5

## Porting software to hardware using XLS/DSLX

[paper](PDFs/2021/a05.pdf)
[presentation](Videos/2021/a05-video.mp4)
[slides](PDFs/2021/a05-slides.pdf)
[repo](https://google.github.io/xls/dslx_reference/)

## Abstract

[DSLX](https://google.github.io/xls/dslx_reference/) is a dataflow-oriented functional language used to build hardware that can also run effectively as host software.

DSLX's syntax resembles Rust, while being an immutable expression-based dataflow DSL and adding hardware-oriented features like arbitrary bitwidths.

Using the [XLS](https://google.github.io/xls/) (Accelerated HW Synthesis) toolchain, DSLX can target to XLS IR intermediate format to enable development flows for FPGAs and ASICs (thru Verilog conversation) or native-speed execution (thru LLVM-based JIT compilation).

In this presentation (submitted in the *"Work in Progress"* category), we go step-by-step thru the process of *"Porting software to hardware"* by rewriting a C routine in DSLX and showing how to integrate the XLS toolchain in a typical FLOSS FPGA flow to synthesize it on a budget FPGA board like the [FoMU](https://tomu.im/fomu.html).

### Aurthors
1. Johan Euphrosine <proppy@google.com> (Google)
2. Rob Springer <rspringer@google.com> (Google)

# Article 6

## MLIR as Hardware Compiler Infrastructure
[paper](PDFs/2021/a06.pdf)
[presentation](Videos/2021/a06-video.mp4)
[slides](PDFs/2021/a06-slides.pdf)
[repo](https://github.com/llvm/circt)

### Abstract

### Authors
1. Schuyler Eldridge <schuyler.eldridge@sifive.com> (SiFive)
2. Prithayan Barua (SiFive)
3. Aliaksei Chapyzhenka (SiFive)
4. Adam Izraelevitz (SiFive)
5. Jack Koenig (SiFive)
6. Chris Lattner (SiFive)
7. Andrew Lenharth (SiFive)
8. George Leontiev (SiFive)
9. Fabian Schuiki (SiFive)
10. Ram Sunder (SiFive)
11. Andrew Young (SiFive)
12. Richard Xia (SiFive)

# Article 7

## A Toolkit for Designing Hardware DSLs
[paper](PDFs/2021/a07.pdf)
[presentation](Videos/2021/a07-video.mp4)
[slides](PDFs/2021/a07-slides.pdf)
[repo](https://calyxir.org/)

### Abstract
Recent years have seen a renewed interest in open-source hardware design tools everywhere in the stack---from new register-transfer-level (RTL) languages to open-source flows for fabricating silicon.  While innovation in the traditional hardware stack promises better, faster, and more portable tools, key innovations are still needed to democratize hardware design.  Specifically, domain specific languages (DSLs) which allow experts to concisely express computations without delving into low-level hardware details are needed to enable widespread use of hardware accelerators.  In order to simplify the gargantuan task of implementing, optimizing, and lowering such hardware domain specific languages (DSLs), we have been building Calyx, an intermediate language (IL) and a compiler infrastructure for accelerator generators.  We demonstrate how Calyx IL's novel separation between the structural and control-flow aspects of an accelerator design enables it to: (1) simplify frontends by efficiently encoding their semantics, (2) enable novel optimization passes that cannot be performed in traditional hardware ILs, and (3) allow us to build software-like debugging infrastructure.

### Authors
1. Griffin Berlstein <griffin@cs.cornell.edu> (Cornell University)
2. Rachit Nigam <rnigam@cs.cornell.edu> (Cornell University)
3. Chris Gyurgyik <cpg49@cornell.edu> (Cornell University)
4. Adrian Sampson <asampson@cs.cornell.edu> (Cornell University)

# Article 8

## Towards Functional Coverage-Driven Fuzzing for Chisel Designs
[paper](PDFs/2021/a08.pdf)
[presentation](Videos/2021/a08-video.mp4)
[slides](PDFs/2021/a08-slides.pdf)
[repo](https://github.com/chiselverify/chiselverify)

### Abstract
Verification of digital systems must be done in ever tighter time constraints due to the rise of domain-specific hardware accelerators. To combat this, we can learn from agile techniques, typical in software engineering, and use them for hardware development. In this mindset, Chisel, a hardware construction language embedded in Scala, was developed as a tool to accelerate the implementation of digital designs. Following this path, we developed a high-level verification library named ChiselVerify, bringing functionalities such as functional coverage to the Chisel ecosystem. Using this tool, we propose a functional coverage-driven mutation-based fuzzer for Chisel designs. Initial experiments are done on the Leros accumulator ALU.

### Author
1. Andrew Dobis <adobis@student.ethz.ch> (Technical University of Denmark)
2. Tjark Petersen <s186083@student.dtu.dk> (Technical University of Denmark)
3. Martin Schoeberl <masca@dtu.dk> (Technical University of Denmark)

# Article 9

## SystemVerilog IDE integration with Verible Language Server support
[paper](PDFs/2021/a09.pdf)
[presentation](Videos/2021/a09-video.mp4)
[slides](PDFs/2021/a09-slides.pdf)
[repo](https://github.com/chipsalliance/verible)

### Abstract
[Verible](https://github.com/chipsalliance/verible) is an Open Source developer productivity tool for SystemVerilog. It provides linting, including auto-fix patches, formatting, and code indexing as well as project inspection tools.

Integration with github actions allows to automatically run in continuous integration and comment on pull requests, helping to improve code quality in development teams.

So far, all of these uses have been offline on files at rest, but tool support while writing the code is an additional way Verible will improve developer productivity. Providing online symbol navigation such as "jump to definition" and code quality feedback directly in the IDE is a newly developed feature of Verible. Using the language server protocol, this feature is compatible with all common IDEs.

In this presentation (submitted in the _Work-in-progress_ category), we will give a hands-on introduction of using the various features of the Verible tool set, including the current state of the IDE integration with the language server protocol.

### Author
Henner Zeller <hzeller@google.com> (Google)

# Article 10

## RTLFuzzLab
[paper](PDFs/2021/a10.pdf)
[presentation](Videos/2021/a10-video.mp4)
[slides](PDFs/2021/a10-slides.pdf)
[repo](https://github.com/ekiwi/rtl-fuzz-lab)

### Abstract
--------
Coverage directed mutational fuzz testing has become a popular tool for automated software testing and bug detection. This technique works by providing inputs to a program and measuring which branches in the program under test are explored during execution of those seed inputs. The fuzzer then automatically mutates the original inputs by applying a series of deterministic and non-deterministic mutation operations. The program under test is ran on these newly generated mutant inputs. A new input will be retained to serve as the start for new mutations if and only if it produces coverage of branches which have not been seen before or significantly increases the times a branch has been covered. The vast majority of mutant inputs are immediately discarded as they do not improve the coverage. This automated fuzzing has been very successful in uncovering countless software bugs, however, it has yet to catch on for testing digital hardware designs.

The initial work on applying the fuzzing algorithm used for software testing to register transfer level (RTL) designs described the various added degrees of freedom that we face in the hardware context [1]. One important decision is how to take the sequence of bytes provided by a software fuzzer and use it in a testbench. The simplest solution is to just apply new data to the input wires of the design under test and to stop the test execution once we run out of data provided by the fuzzer. More recent work has proposed to instead covert the raw bytes into read or write tile link transactions through the use of a grammar [2]. Another question is what coverage metric to use as feedback to the fuzzer. The original paper counted the number of toggles on a multiplexer control signal [1], while subsequent papers have suggested to only count full toggles [3] or to use the branch coverage of a software simulation model as proxy for line coverage of the RTL description [2]. The choice of initial input seeds to begin fuzzing with can also affect the results.

We present our ongoing work on RTLFUZZLAB, an open-source framework based on the FIRRTL RTL compiler infras-tructure [4], that makes it easy to explore new fuzzing ideas. We provide an easy integration of the popular AFL fuzzer and are working on adding our own fuzzer implementation to be able to experiment with custom mutations and fuzz scheduler designs. Our direct harness is based on the ideas from the Rfuzz paper [1] and works on any RTL circuit with a single input clock and reset. It can be easily switched out for a bus-centric harness which re-implements the tile link specific harness from the work on Fuzzing hardware like software [2]. We provide various coverage metrics like mux toggle coverage [1], full mux toggle coverage [3] and HDL line coverage (approximating the coverage used in [2]). These coverage metrics can be combined with post-processing functions and arbitrary combinations of them can be selected as feedback to the fuzzer. We also include some simple benchmarks as well as scripts to run benchmarks and analyze results, making it easy to prototype new fuzzing ideas. The code is open source under a BSD license and available on GitHub: https://github.com/ekiwi/rtl-fuzz-lab

REFERENCES

[1] K. Laeufer, J. Koenig, D. Kim, J. Bachrach, and K. Sen, “Rfuzz: Coverage-directed fuzz testing of rtl on fpgas,” in 2018 IEEE/ACM International Conference on Computer-Aided Design (ICCAD). IEEE, 2018, pp. 1–8.

[2] T. Trippel, K. G. Shin, A. Chernyakhovsky, G. Kelly, D. Rizzo, and M. Hicks, “Fuzzing hardware like software,” arXiv preprint arXiv:2102.02308, 2021.

[3] T. Li, H. Zou, D. Luo, and W. Qu, “Symbolic simulation enhanced coverage-directed fuzz testing of rtl design,” in 2021 IEEE International Symposium on Circuits and Systems (ISCAS). IEEE, 2021, pp. 1–5.

[4] A. Izraelevitz, J. Koenig, P. Li, R. Lin, A. Wang, A. Magyar, D. Kim, C. Schmidt, C. Markley, J. Lawson et al., “Reusability is FIRRTL Ground: Hardware Construction Languages, Compiler Frameworks, and Transformations,” in 2017 IEEE/ACM International Conference on Computer-Aided Design (ICCAD). IEEE, 2017, pp. 209–216.

### Authors

1. Brandon Fajardo <brfajardo@berkeley.edu> (UC Berkeley)
2. Kevin Laeufer <laeufer@berkeley.edu> (UC Berkeley)
3. Jonathan Bachrach <jrb@berkeley.edu> (UC Berkeley)
4. Koushik Sen <ksen@berkeley.edu> (UC Berkeley)

# Article 11

## A CMOS Programmable Analog Standard Cell Library in Skywater 130nm Open-Source Process
[paper](PDFs/2021/a11.pdf)
[presentation](Videos/2021/a11-video.mp4)
[slides](PDFs/2021/a11-slides.pdf)
[repo](https://gitlab.com/um-ece/ftl-lab/hilas)

### Abstract

This work presents an implemented, and where allowed, openly-available programmable analog standard cell library in the open-source skywater 130nm bulk CMOS processes. Standard CMOS elements enable programmablility for many standard-cell components, eliminating the need for large number of device geometries required in classic analog design.    This effort presents the methodology in developing these analog standard cell library. The standard cell library was designed to integrate with digital open-source synthesis tools.

### Authors

1. Jennifer Hasler <jennifer.hasler@ece.gatech.edu> (Georgia Institute of Technology)
2. Barry Muldrey <muldrey@olemiss.edu> (University of Mississippi)
3. Parker Hardy <pwhardy@go.olemiss.edu> (University of Mississippi)

# Article 12

## LSOracle 2.0: Capabilities, Integration, and Performance
[paper](PDFs/2021/a12.pdf)
[presentation](Videos/2021/a12-video.mp4)
[slides](PDFs/2021/a12-slides.pdf)
[repo](https://github.com/lnis-uofu/LSOracle)

### Abstract
LSOracle is a tool for logic synthesis which uses several directed acyclic graph representations concurrently when optimizing a design; for example a combination of And-Inverter Graphs and Majority-Inverter Graphs. Version 2.0 of LSOracle has recently been released. This paper describes the changes made in version 2.0 and presents recent benchmark results compared to earlier versions of the tool. Execution time has been reduced by a factor of ten with an accompanying 5-10\% improvement in area-delay product.

### Authors
1. Scott Temple <scott.temple@utah.edu> (University of Utah)
2. Ashton Snelgrove <ashton.snelgrove@utah.edu> (University of Utah)
3. Walter Lau Neto <walter.launeto@utah.edu> (University of Utah)
4. Pierre-Emmanuel Gaillardon <pierre-emmanuel.gaillardon@utah.edu> (University of Utah)

# Article 13

## interact: An Interactive Design Environment for Asynchronous Logic
[paper](PDFs/2021/a13.pdf)
[presentation](Videos/2021/a13-video.mp4)
[slides](PDFs/2021/a13-slides.pdf)
[repo](http://github.com/asyncvlsi/interact)

### Abstract

We are developing an open-source EDA flow for asynchronous logic. We present the current state of the flow, where all the key components have been integrated into a single framework including the timer, partitioner, placer, power detailed router, and global router. We describe enhancements to the flow in terms of the class of circuits that can be handled, and extensions to support third-party libraries and flows.

### Authors

1. Jiayuan He <hejy@cs.utexas.edu> (University of Texas at Austin)
2. Wenmian Hua <wenmian.hua@yale.edu> (Yale University)
3. Yi-Shan Lu <yishanlu@cs.utexas.edu> (University of Texas at Austin)
4. Sepideh Maleki <smaleki@cs.utexas.edu> (University of Texas at Austin)
5. Yihang Yang <yihang.yang@yale.edu> (Yale University)
6. Keshav Pingali <pingali@cs.utexas.edu> (University of Texas at Austin)
7. Rajit Manohar <rajit.manohar@yale.edu> (Yale University)

# Article 14

## Towards Fast and Accurate Parallel Chip Thermal Simulations with PACT
[paper](PDFs/2021/a14.pdf)
[presentation](Videos/2021/a14-video.mp4)
[slides](PDFs/2021/a14-slides.pdf)
[repo](https://github.com/peaclab/PACT)

### Abstract

Over the last few decades, chip temperature has become one of the most important criteria for designing high-performance, cost-effective, and reliable integrated circuits (ICs). Increased power consumption and temperature not only degrade the performance of a chip but also generate larger sub-threshold leakage power and cause reliability challenges. Therefore, thermal analysis is an essential procedure for designing any chip. Conventional thermal analysis relies on finite-element method (FEM) based multiphysics simulators (e.g., COMSOL and ANSYS). Such commercial simulators are computationally expensive and experience long solution times along with large memory requirements. These limitations make commercial simulators unsuitable for evaluating numerous design alternatives or runtime scenarios. Therefore, having fast and accurate thermal analysis is crucial for chip design and thermal optimization. In this paper, we discuss the key features of a SPICE-based PArallel Compact Thermal simulator (PACT) that achieves fast and accurate, standard-cell to architecture-level, steady-state and transient parallel thermal simulations.

### Authors

1. Zihao Yuan <yuan1z@bu.edu> (Boston University)
2. Prachi Shukla <prachis@bu.edu> (Boston University)
3. Sofiane Chetoui <sofiane_chetoui@brown.edu> (Brown university)
4. Carlton Knox <cknox@bu.edu> (Boston University)
5. Sean Nemtzow <snemtzow@bu.edu> (Boston University)
6. Sherief Reda <sherief_reda@brown.edu> (Brown University)
7. Ayse K. Coskun <acoskun@bu.edu> (Boston University)

# Article 15

## FABulous: an Open-Everything Framework for Embedded FPGAs
[paper](PDFs/2021/a15.pdf)
[presentation](Videos/2021/a15-video.mp4)
[slides](PDFs/2021/a15-slides.pdf)
[repo](https://github.com/FPGA-Research-Manchester/)

### Abstract
This paper presents the open-source embedded FPGA framework FABulous that is designed for ease-of-use and excellent quality of results in terms of logic density, performance, and power consumption. FABulous users can build a fabric from predefined tiles for logic, memory, arithmetic, and various IO. The tiles are stitched together in a Lego-like manner, as needed.
Users can add custom tiles or customize the routing resources and most architectural details of the FPGA fabrics. Experienced designers can provide optimized cells for configuration storage or switching (e.g., pass transistor multiplexers, what we currently provide for TSMC 180nm and Skywater 130nm). Alternatively, FABulous can fall back to a standard cell design, which makes FABulous FPGAs easily portable across different technology nodes.
Fabulous comes with unique features that are not available in other open-source FPGA frameworks like low power frame-wise reconfiguration and dynamic partial configuration. FABulous integrates several other open-source projects (Yosys, nextpnr, VPR, OpenLane, Verilator) to provide a full and open end-to-end user experience.

### Authors

1. Bea Healy <tabitha.healy@student.manchester.ac.uk> (University of Manchester)
2. Jing Yu <jing.yu@manchester.ac.uk> (University of Manchester)
3. Nguyen Dao <nguyen.dao@manchester.ac.uk> (University of Manchester)
4. King Lok Chung <king.chung@student.manchester.ac.uk> (University of Manchester)
5. Dirk Koch <dirk.koch@manchester.ac.uk> (University of Manchester)

# Article 16

## Software Inspired IC Hardware Workflows Using Bazel
[paper](PDFs/2021/a16.pdf)
[presentation](Videos/2021/a16-video.mp4)
[slides](PDFs/2021/a16-slides.pdf)
[repo](https://github.com/hdl/bazel_rules_hdl)

### Abstract

Over the past 20 years a significant amount of development has gone into developer tooling to build software safely, and repeatedly. \emph{Bazel} is an open source build system designed from the ground up to accommodate highly variable language tool chains and massive software builds. This project aims to leverage that very same technology to offer software inspired workflows to build integrated circuits.

In this abstract session, I discuss the open source project [hdl/bazel_rules_hdl](https://github.com/hdl/bazel_rules_hdl) which aims to use \emph{Bazel}, \emph{OpenROAD} , \emph{Yosys} and other open source tools to build a software like workflow that integrates synthesis, place and route, and verification into well defined build rule functions that can be easily run, distributed, and cached on multiple machines using the existing capabilities of Bazel.

Today `hdl/bazel_rules_ hdl` offers Bazel rules that will synthesize, place and route and run regression tests against the final placed and routed design. The regression tests allow you to set power and area thresholds on subblocks that cannot be exceeded without updating the thresholds, or modifying the problematic RTL.

These build rules give you the ability to setup software like presubmits that prevent RTL modifications that reduce the final PPA of the design, break the place and route or negatively impact synthesis. These types of workflows are common in the software model, but are novel in the hardware workflow space.

The long term goal of this project is that it enables users to run `bazel test //mychip/...` and `bazel build //mychip:gds` and in 10 minutes you have verified and emitted a fabricatable IC even for the most complex designs.

### Author
Ethan Mahintorabi <ethanmoon@google.com> (Google)

# Article 17

## Vezzal - a containerized tool to work with and test open source EDA tools
[paper](PDFs/2021/a17.pdf)
[presentation](Videos/2021/a17-video.mp4)
[slides](PDFs/2021/a17-slides.pdf)
[repo](https://github.com/masc-ucsc/livehd)

### Abstract
Constant development of tools often breaks something internally which can lead to other issues. Hence there is a need to test the tool for its previous supporting features. But the tool needs an environment to get launched and good test cases to test the features. This problem can be solved by "Vezzal". It is a docker containerised environment which is built completely from scratch, as shown in figure 1, which can be operated in two modes - user mode and test mode. In the test mode of Vezzal, the tool is provided with an environment supporting all dependencies like compilers, libraries etc., and a test cases database which could test the tool its core and supporting features with a very few inputs from the user. The testing can be done through the GitHub Actions feature to trigger the Vezzal because of any changes to the tool, thus supporting the continuous integration (CI) of tools. The CI workflow is shown in figure 2. Currently, the Vezzal is supporting the CI for Magic and Netgen tools at a basic level. In the user mode, Vezzal can be used to work with the supporting open-source EDA tools without worrying about the tool dependencies and can exercise them using the test cases database as examples. In addition to the main goal, Vezzal is designed to keep everything simple by following the KISS (KEEP IT SIMPLE, STUPID) principle to avoid any kind of usage restrictions, giving complete freedom to mould Vezzal according to the needs and requirements of the user. The CI feature offered by Vezzal couldn't be possible without the docker technology, which is also employed by the OpenLane, and GitHub Actions. Many other tools will be added under user mode soon

### Author
Sai Charan Lanka <lankasaicharan@ieee.org> (None)

# Article 18

Removed.

# Article 19

## Developing Open-Source Circuit Design and Flow Management Software
[paper](PDFs/2021/a19.pdf)
[presentation](Videos/2021/a19-video.mp4)
[slides](PDFs/2021/a19-slides.pdf)
[repo](http://www.opencircuitdesign.com/open_pdks)

### Abstract
The need for open-source tools for circuit design for custom silicon hardware has increased since the establishment of the Skywater open-source process design kit (PDK). This project aims to improve and extend existing software tools and scripts that help users with developing circuits; and to migrate the tools, which currently are mostly on the Efabless, Inc. platform, to a platform-independent, open environment. The project's end goal is to improve the functionality of an existing project manager and provide intuitive software for managing circuit design flows. The flow manager guides users through a specific design process, integrating the PDK and tools and ensuring that all conditions are being met in the process. The project aims to support the analog, design, mixed-signal, and chip assembly flows, each of which has its own unique set of tools and steps.

### Authors
1. Maxwell Chen <maxwellfchen@gmail.com> (Poolesville High School)
2. R. Timothy Edwards <tim@efabless.com> (Efabless)

# Article 20

## A Parallel HDL Compilation Framework
[paper](PDFs/2021/a20.pdf)
[presentation](Videos/2021/a20-video.mp4)
[slides](PDFs/2021/a20-slides.pdf)
[repo](https://github.com/masc-ucsc/livehd)

### Abstract
We present LiveHD, a parallel HDL compiler to boost the HDL compilation
throughput. The hierarchical dependency of the design is resolved internally in
LiveHD without any pre-scan step on source files. We identify why and how LiveHD pass is compiled with full parallelism or a bottom-up scheme by referencing the design dependency relation. Our results show that when compiling the highest level of FIRRTL language, CHIRRTL, LiveHD is 1.7x faster than the FIRRTL compiler with single-threaded; and 3.1 to 5.48X faster when exploiting 2-5 threads.

### Author
1. Sheng-Hong Wang <swang203@ucsc.edu> (University of California, Santa Cruz)
2. Sakshi Garg <sgarg3@ucsc.edu> (University of California, Santa Cruz)
3. Hunter James Coffman <hcoffman@ucsc.edu> (University of California, Santa Cruz)
4. Kenneth Mayer <krmayer@ucsc.edu> (University of California, Santa Cruz)
5. Jose Renau <renau@ucsc.edu> (University of California, Santa Cruz)

# Article 21

## OpenCache: An Open-Source OpenRAM Based Cache Generator
[paper](PDFs/2021/a21.pdf)
[presentation](Videos/2021/a21-video.mp4)
[slides](PDFs/2021/a21-slides.pdf)
[repo](https://github.com/VLSIDA/OpenCache)

### Abstract
--------
Hardware caches are used in order to maximize the average latency of large memory blocks. The client logic is usually a CPU core but it may well be an application specific logic. However, designing a cache manually from scratch is difficult. In this paper, we describe OpenCache, an open-source parameterized IP core generator. OpenCache calls OpenRAM on the fly, while considering OpenRAM efficiency issues. The current version of OpenCache supports a single pipelined and in-order read-write port on the client side. It outputs a synthesizable Verilog module for cache logic and configuration files for OpenRAM to compile internal SRAM blocks holding data and tags of the generated cache.

### Authors
1. Eren Dogan <eren.dogan@ozu.edu.tr> (Ozyegin University)
2. Hasan Fatih Ugurdag <fatih.ugurdag@ozyegin.edu.tr> (Ozyegin University)
3. Matthew Guthaus <mrg@ucsc.edu> (UC Santa Cruz)

# Article 22

## A Guide for Rapid Creation of New HDLs
[paper](PDFs/2021/a22.pdf)
[presentation](Videos/2021/a22-video.mp4)
[slides](PDFs/2021/a22-slides.pdf)
[repo](https://github.com/masc-ucsc/livehd)

### Abstract
We present a guide for quickly building and testing a new HDL. Upcoming HDLs have a compiler designed specifically for each of them, which means duplicated efforts. The proposed guidelines minimize these efforts. New language developers can leverage existing compiler infrastructures to interface with the new HDL. This interfacing would enable developers to use LEC without any reference compiler. The proposed method also leads to converting the newly developed HDL to any other language supported by the interfaced compiler. Also, this system would ensure higher trust in the language and the interfaces.

### Authors

1. Sakshi Garg <sgarg3@ucsc.edu> (University of California, Santa Cruz)
2. Sheng-Hong Wang <swang203@ucsc.edu> (University of California, Santa Cruz)
3. Hunter James Coffman <hcoffman@ucsc.edu> (University of California, Santa Cruz)
4. Jose Renau <renau@ucsc.edu> (University of California, Santa Cruz)

# Article 23

## ESSENT: A High-Performance RTL Simulator
[paper](PDFs/2021/a23.pdf)
[presentation](Videos/2021/a23-video.mp4)
[slides](PDFs/2021/a23-slides.pdf)
[repo](https://github.com/ucsc-vama/essent)

### Abstract
RTL simulation is a critical tool for hardware development, debugging, design space exploration, and verification. The slow speed of hardware simulation can often be a bottleneck for the design process, so any speed improvements could either reduce design times or improve design quality. We overview ESSENT, a high-performance RTL simulator available as open-source. Not only does it contain novel optimizations that make it typically faster than other software RTL simulators, the codebase can serve as a foundation for simulation research.

### Authors
1. Scott Beamer <sbeamer@ucsc.edu> (UC Santa Cruz)
2. Thomas Nijssen <tnijssen@ucsc.edu> (UC Santa Cruz)
3. Krishna Pandian <kpandian@ucsc.edu> (UC Santa Cruz)
4. Kyle Zhang <kmzhang@ucsc.edu> (UC Santa Cruz)
