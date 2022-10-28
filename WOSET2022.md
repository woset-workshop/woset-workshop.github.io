#  WOSET 2022 Proceedings

To cite an article, please use this format:
(author names here), "(article title here)", Article No. (article number here), Workshop on Open-Source EDA Technology (WOSET), 2022.

For live discussions via Zoom and Slack, please see the [WOSET 2022 Schedule](WOSET2022-schedule.md).

## Organization

### Co-Chairs
* Jose Renau, UC Santa Cruz (Co-Chair)
* Matthew Guthaus, UC Santa Cruz (Co-Chair)

### Program Committee
* Matthew Guthaus, UC Santa Cruz
* Jose Renau, UC Santa Cruz
* Matthew Venn, YosysHQ & ChipFlow
* Rajit Manohar, Yale University
* Scott Temple, University of Utah
* Jonathan Balkind, UC Santa Barbara
* Tobias Grosser, University of Edinburgh

### Web Chairs
* Jesse Cirimeli-Low, UC Santa Cruz
* Sakshi Garg, UC Santa Cruz

# Article 1

## Open source FPGA-based emulation with Nexus
[paper](PDFs/2022/1-Birch-paper.pdf)
[presentation (long)](Videos/2022/1-Birch-long.mp4)
[presentation (short)](Videos/2022/1-Birch-short.mp4)
[slides](PDFs/2022/1-Birch.pdf)
[repo](https://github.com/intuity/nexus)

### Abstract
Nexus is a hardware-accelerated emulation platform for small designs at simulated clock rates approaching 1 MHz. The solution is split into a parameterisable systolic array targeting FPGA fabrics, and a specialised compiler which partitions a design and generates instruction streams for each node in the array. This paper explains the problem and details the development of the hardware and the compiler. The complete source code is published on GitHub with a permissive Apache-2.0 license.

### Authors
1. Peter Birch (Unaffiliated) <peter@intuity.io>

# Article 2

## Accelerate Silicon Design with Jupyter Notebooks
[paper](PDFs/2022/2-Euphrosine.pdf)
[presentation (long)](Videos/2022/2-Euphrosine-long.mp4)
[presentation (short)](Videos/2022/2-Euphrosine-short.mp4)
[repo](https://github.com/proppy/rad-lab)

### Abstract
In this Work in Progress session we showcase our recent work to leverage Jupyter Notebooks and Conda packages to publish and share interactive silicon design experiments.

Notebooks published at https://github.com/chipsalliance/silicon-notebooks demonstrate how run a design experiment from design to gds using publicly-hosted notebooks without having to install any tool locally.

Additionally we show how those notebooks can be scaled on a public cloud provider to explore the parameters space of various silicon designs:

We deploy an opensource terraform solution https://github.com/proppy/rad-lab to provision jupyter notebooks with all the necessary tools pre-installed to model our experiments w/ design and flow parameters.
Between each batch of experiments we report estimated performance metrics to a blackbox and hyperparameter optimization service (which has also an opensource implementation https://github.com/google/vizier) allowing it to suggest new parameters for future batches.
We observe that the experiments quickly converge toward the best metrics for the given designs.
Each of the jobs result in a standalone notebook allowing us to share, aggregate and reproduce every experiments.

### Authors
1. Johan Euphrosine (Google) <proppy@google.com>

# Article 3

## SODA Synthesizer: an Open-Source, End-to-End Hardware Compiler
paper
presentation (long)
presentation (short)
slides
repo

### Abstract
Enabling autonomous control in novel scientific experimental workflows requires the ability to generate highly specialized systems for data analysis and artificial intelligence, enabling the low-latency reasoning capabilities needed to take real-time decisions. %Novel "converged" applications combine phases of scientific simulation with data analysis and machine learning. Each computational phase can benefit from specialized accelerators. However, algorithms evolve so quickly that mapping them on existing accelerators is suboptimal or even impossible. This paper presents the SODA (Software Defined Accelerators) framework, an open-source modular, multi-level, no-human-in-the-loop, hardware compiler that enables end-to-end generation of specialized accelerators from high-level data science frameworks. SODA is composed of SODA-Opt, a high-level frontend developed in MLIR that interfaces with domain-specific programming environments and allows performing system level design, and Bambu, a state-of-the-art high-level synthesis (HLS) engine that can target different device technologies. The framework implements design space exploration as compiler optimization passes. We show how the modular, yet tight, integration of the high-level optimizer and lower-level HLS tools enables the generation of accelerators optimized for the computational patterns of converged applications. We then discuss some of the research opportunities that such an open-source framework allows.

### Authors
1. Nicolas Bohm Agostini (Pacifici Northwest National Laboratory) <nicolas.agostini@pnnl.gov>
2. Serena Curzel (Politecnico di Milano) <serena.curzel@polimi.it>
3. Ankur Limaye (Pacifici Northwest National Laboratory) <ankur.limaye@pnnl.gov>
4. Vinay Amatya (Pacific Northwest National Laboratory) <vinay.amatya@pnnl.gov>
5. Marco Minutoli (Pacific Northwest National Laboratory) <marco.minutoli@pnnl.gov>
6. Vito Giovanni Castellana (Pacific Northwest National Laboratory) <vitogiovannicastellana@pnnlgov>
7. Joseph Manzano (Pacific Northwest National Laboratory) <joseph.manzano@pnnl.gov>
8. Fabrizio Ferrandi (Politecnico di Milano) <fabrizio.ferrandi@polimi.it>
9. Antonino Tumeo (Pacific Northwest National Laboratory) <antonino.tumeo@pnnl.gov>

# Article 4

## Bitstream Chef
[paper](PDFs/2022/4-Kashif.pdf)
[presentation](Videos/2022/4-Kashif.mp4)
[slides](PDFs/2022/4-Kashif-slides.pdf)
[repo](https://github.com/shahzaibk23/Bitstream-Chef)

### Abstract
Electronic Design Automation (EDA) technologies have become increasingly important in their fields of application with the open-source revolution in the silicon industry. These tools cover a wide range of automatic operations that save a significant amount of time. Bitstream Chef generates the bitstream of a design as shown in Fig.1 by taking an RTL design, allowing the user to map I/Os onto an FPGA using a GUI, and thus generating the bitstream through automated processes by use of an open-source tool F4PGA. Additionally, it uploads the Bitstream onto the connected FPGA board while also letting the user know whether any boards are currently connected. It will also allow user to either have pre-defined program embedded in the bitstream or upload the program separately through UART. For further moving the design toward GDS generation, it has the Open Lane toolchain integrated as well. Bitstream Chef is designed to be the go-to tool for every developer who frequently must upload or burn designs into FPGA, has a computer with less computing power.

### Authors
1. Shazaib Kashif (Usman Institute of Technology) <shazaib@students.uit.edu>
2. Talha Ahmed (Usman Institute of Technology) <tahmed@students.uit.edu>
3. Farhan Ahmed Karim (Universiti Kebangsaan Malaysia) <faahmed@uit.edu>

# Article 5

## Accessibility of Chip Design to the Non-Professional
paper
[presentation](Videos/2022/5-Goldstein.mp4)
[slides](PDFs/2022/5-Goldstein.pdf)
[repo](https://github.com/AlexanderJGoldstein/chaos_automaton_Summer_2022)

### Abstract
Over the summer of 2022, Alexander Goldstein worked under the mentorship of Tim Edwards to test both the usability and accessibility of modern day open source EDA tools and methods for chip design. To test how easily EDA technology could be used by the general public, the authors prepared a design for the Open Source MPW-7 Shuttle by Efabless. The process of creating the final layout from the verilog source code proved to be more efficient and accessible than initially expected, but also surfaced potential shortcomings and limitations within the software. This report discusses the pros and cons of issues such as system memory and performance requirements, clarity of documentation and reference examples, and the restriction to a Linux-based environment. Overall, this research has proved that it is possible for a high school student to effectively use current EDA technologies, which will allow more people to enter the Electronic Design space.

### Authors
1. Alexander Goldstein (Poolesville High School) <Alex_Goldstein@outlook.com>
2. Tim Edwards (Open Circuit Design, efabless.com) <tim@opencircuitdesign.com>

# Article 6

## SoC-Now: An Open-Source Web based RISC-V SoC Generator
[paper](PDFs/2022/6-Shahzaib.pdf)
[presentation](Videos/2022/6-Shahzaib.mp4)
[slides](PDFs/2022/6-Shahzaib-slides.pdf)
[repo](socnow.software)

### Abstract
In the rapidly changing technological world of today, smart phones and other gadgets have taken over our daily lives. Every aspect of life is reliant on technology, or "smart devices." And these devices are called “smart” because they contain a computing system inside called as processor or system on chip (SoC). Development of SoC is a quite long process. It can take months to build and develop a SoC from scratch. Following the design stage, testing, and verification of it adds another layer of stress. Designers like to reuse a verified component in their design to save time. However, this doesn't save time because without adequate documentation, which is lacking in many contributions to open-source projects, it can be extremely challenging to grasp the functionality and usability of a component. The open-source semiconductor industry is therefore in need of software that can quickly produce or design a SoC rather than taking the designer years to complete the build or design. Alternately, any designer can also generate a component with sufficient documentation and plug and play support. SoC-Now is an open-source web-based RISC-V ISA [1][2][3] standardised SoC design solution in terms of generator that enables anyone to create a SoC with their own customised specifications and then further process that SoC to the Field Programmable Gate Array (FPGA) Emulation. Additionally, it provides the capability to produce any standalone, verified, and reusable SoC component (Core, Device, Bus) by means of generic interfaces. A completely automated Verification system is also included.

### Authors
1. Muhammad Shahzaib (Usman Institute Of Technology) <mshahzaib@students.uit.edu>
2. Shahzaib Kashif (Usman Institute Of Technology) <shahzaib@students.uit.edu>
3. Talha Ahmed (Usman Institute Of Technology) <tahmed@students.uit.edu>
4. Farham Ahmed Karim (Universiti Kebangsaan Malaysia) <faahmed@uit.edu>

# Article 7

## TensorLib: A Spatial Accelerator Generation Framework for Tensor Algebra
paper
[presentation](Videos/2022/7-jia.mp4)
[slides](PDFs/2022/7-jia.pdf)
[repo](https://github.com/pku-liang/TensorLib)

### Abstract
Tensor algebra finds applications in various domains, and these applications, especially when accelerated on spatial hardware accelerators, can deliver high performance and low power. This paper proposes TensorLib, a framework for generating spatial hardware accelerators for tensor algebra applications. TensorLib is motivated by the observation that, different dataflows share common hardware modules, which can be reused across different designs. To build such a framework, TensorLib first uses Space-Time Transformation to explore different dataflows, which can compactly represent the hardware dataflow using a simple transformation matrix. Next, we identify the common structures of different dataflows and build parameterized hardware module templates with Chisel. Our generation framework can select the needed hardware modules for each dataflow, connect the modules using a specified interconnection pattern, and automatically generate the memory and controller architecture for a complete hardware accelerator design. TensorLib remarkably improves the productivity for developing and optimizing spatial hardware architecture. It provides a Scala-based DSL for users to efficiently define tensor computation and dataflow parameters. The framework is written in Chisel hardware construction language to generate Verilog source code for the accelerator.

### Authors
1. Liancheng Jia (Peking University) <jlc@pku.edu.cn>
2. Zizhang Luo (Peking University) <semiwaker@pku.edu.cn>
3. Liqiang Lu (Peking University) <liqianglu@pku.edu.cn>
4. Yun Liang (Peking University) <ericlyun@pku.edu.cn>

# Article 8

## OpenRegFile: Open-Source Register File Generation
[paper](PDFs/2022/8-Ahmed.pdf)
[presentation](Videos/2022/8-Ahmed.mp4)
slides
[repo](https://github.com/VLSIDA/OpenRAM)

### Abstract
This work presents an extension of the OpenRAM memory compiler to provide the automated generation of latch-based register files. It uses standard cells from the Skywater 130nm library. OpenRegFile automatically generates a spice netlist, layout, and a verilog model. It leverages the hierarchical decoders and muxes from SRAM designs. The cells for the decoders and muxes in SRAMs are custom made but we replace them with standard cells to improve routability and portability to other technologies with a cell library. At first, we created a register file array along with a tristate. The tristate helps to use the same data-line throughout the array of D-Latches which improves routing. We used the spice netlist API to implement the logic in OpenRAM and created custom modules to create the layout.

### Authors
1. Talha Ahmed (Usman Institute Of Technology) <tahmed@students.uit.edu>
2. Jesse Cirimelli-Low (University of California, Santa Cruz) <jcirimel@ucsc.edu>
3. Matthew Guthaus (University of California, Santa Cruz) <mrg@ucsc.edu>

# Article 9

## xcell: a cell library characterizer for combinational and state-holding gates
[paper](PDFs/2022/9-Manohar-paper.pdf)
[presentation](Videos/2022/9-Manohar-short.mp4)
[slides](PDFs/2022/9-Manohar.pdf)
[repo](https://github.com/asyncvlsi/xcell)

### Abstract
We present an open-source cell library characterizer suitable for characterizing combinational logic as well as general state-holding gates that are used in asynchronous logic as well as clocked circuit families like pre-charged logic. The output of the characterizer uses the Synopsys .lib format, and has been used as the input to an existing asynchronous static timing and power analysis tool for multiple technologies and multiple cell libraries.

### Authors
1. Rajit Manohar (Yale University) <rajit.manohar@yale.edu>

# Article 10

## GreenRio: A Modern RISC-V Microprocessor Completely Designed with An Agile Open-source EDA Flow
[paper](PDFs/2022/10-Zhu-paper.pdf)
[presentation (long)](Videos/2022/10-Zhu-long.mp4)
[slides](PDFs/2022/10-Zhu-paper.pdf)
[repo](https://github.com/b224hisl/rioschip)

### Abstract
The booming open-source EDA ecosystem brings transparency and reproducibility to VLSI field, lowering the threshold for CPU design. To facilitate a reliable chip manufacturing flow and prepare for future agile development, we constructed a full-stack design methodology for modern processors in an open-source mode based on our experience in the efabless MPW-7 shuttle (https://github.com/b224hisl/rioschip). We developed a 64-bit dual-issue, out-of-order RISC-V microprocessor “GreenRio”, and completed the back-end process of “RTL-Verification-GDS-Signoff” purely depending on the open-source EDA toolchain. In this paper, we analyzed multiple open source EDA tools from ASIC front-end to back-end. We also proposed some innovations and adaptations based on existing open resources. Moreover, we compared commercial and open-source EDA tools from a modern processor design perspective, with the limitations and future optimizations of the open-source tool summarized. We hope our methodology can help to shed new light upon agile modern architecture development.

### Authors
1. Yifei Zhu (RIOS Lab, TsingHua University) <yifei.z@rioslab.org>
2. Guohua Yin (RIOS Lab, TsingHua University) <guohua.y@rioslab.org>
3. Xinze Wang (RIOS Lab, TsingHua University) <xinze.w@rioslab.org>
4. Zhangxi Tan (RIOS Lab, TsingHua University) <xtan@rioslab.org>

# Article 11

## A Java Backend for ESSENT
paper
[presentation (long)](Videos/2022/11-Eriksson-long.mp4)
[slides](PDFs/2022/11-Eriksson.pdf)
[repo](https://github.com/ekiwi/essent/tree/java-backend)

### Abstract
We propose a new open-source RTL simulator that achieves faster compilation and startup speed compared to compiled simulators, such as Verilator, but also achieves higher simulation performance than interpreted simulators, such as treadle. We build on the work in ESSENT, an optimizing open-source FIRRTL simulator, which has an existing C++ backend, and extend it with a new Java backend. We take advantage of fast Java bytecode compilation and the JVM’s JIT compilation to simultaneously deliver fast simulator startup time and high simulation throughput.

### Authors
1. Augie Eriksson (University of California, Berkeley) <raeriksson@berkeley.edu>
2. Maanuj Vora (University of California, Berkeley) <maanujvora@berkeley.edu>

# Article 12

## Morpher: An Open-Source Integrated Compilation and Simulation Framework for CGRA
[paper](PDFs/2022/12-Wijerathne-paper.pdf)
[presentation (long)](Videos/2022/12-Wijerathne-long.mp4)
[presentation (short)](Videos/2022/12-Wijerathne-short.mp4)
[slides](PDFs/2022/12-Wijerathne-presentation.pdf)
[repo](https://github.com/ecolab-nus/morpher)

### Abstract
This paper presents Morpher, an open-source end-to-end compilation and simulation framework, to assist design space exploration and application-level developments of CGRA-based systems. Morpher can take an application with a compute-intensive kernel as input, compile the kernel onto a user-provided CGRA architecture, and automatically validate the compiled kernels through cycle-accurate simulation using test data extracted from the application. Morpher can handle real-world application kernels without being limited to simple toy kernels through its feature-rich compiler. Morpher architecture description language lets users easily specify architectural features such as complex interconnects, multi-hop routing, and memory organizations. In the experimental study, we evaluate Morpher against state-of-the-art and demonstrate Morpher's ability to provide end-to-end compilation, simulation, and validation. Morpher is available online at https://github.com/ecolab-nus/morpher.

### Authors
1. Dhananjaya Wijerathne (National University of Singapore) <dmd@comp.nus.edu.sg>
2. Zhaoying Li (National University of Singapore) <zhaoying@comp.nus.edu.sg>
3. Manupa Karunarathne (Advanced Micro Devices, Inc.) <Manupa.Karunaratne@amd.com>
4. Tulika Mitra (National University of Singapore) <tulika@comp.nus.edu.sg>
5. Li-Shiuan Peh (National University of Singapore) <peh@comp.nus.edu.sg>

# Article 13

## From Chisel to Chips with Open-Source Tools
[paper](PDFs/2022/13-Schoeberl-paper.pdf)
[presentation](Videos/2022/13-Schoeberl.mp4)
[slides](PDFs/2022/13-Schoeberl-poster.pdf)
[repo](https://github.com/os-chip-design)

### Abstract
Chisel and Verilator provide an open-source stack for digital design. For ASIC synthesis, we have open-source tools like OpenROAD, Yosys, and Magic. OpenROAD is a project to deliver an end-to-end silicon compiler in open source. The aim is to "democratize hardware design" by providing an automated layout generation flow from a design in RTL to GDS files used to produce silicon. Google and Efabless offer free production of chips in a multi-project wafer if the project is available in open source. In this paper, we report our experience in using the open-source tool flow from Chisel to chips with two designs: a small processor using only on-chip resources and a RISC-style processor with extra external main memory. We have successfully taped out both processors for the multi-project waver MPW7 from Efabless.

### Authors
1. Martin Schoeberl (Technical University of Denmark) <masca@dtu.dk>
2. Luca Pezzarossa (Technical University of Denmark) <lpez@dtu.dk>

# Article 14

## Library characterizer for open-source VLSI design
[paper](PDFs/2022/14-Nishizawa-paper.pdf)
[presentation (long)](Videos/2022/14-Nishizawa-long.mp4)
[slides](PDFs/2022/14-Nishizawa.pdf)
[repo](https://github.com/snishizawa/libretto)

### Abstract
This paper introduce an open source cell library characterizer. Free and open-sourced silicon design communities are attracted by hobby designers, academies and industries, and these open-sourced silicon designs are supported by free and open sourced EDAs. However, in our knowledge, tool-chain lacks cell library characterizer. This paper introduce our on-going open source cell library characterizer which can generate timing models and power models of standard cell library.

### Authors
1. Shinichi Nishizawa (Waseda University) <nishizawa@aoni.waseda.jp>
2. Toru Nakura (Fukuoka University) <nakura@fukuoka-u.ac.jp>

# Article 15

## 8bitworkshop: An Interactive Verilog Learning Tool
paper
presentation
slides
repo

### Abstract
8bitworkshop is a web-hosted Interactive Development Environment (IDE) focused on low-level programming of classic 8-bit microcomputers and game consoles. It also has a Verilog simulator, which allows experimentation with simple designs.

The user writes Verilog RTL (Register Transfer Language) source code in the browser-based editor. The IDE compiles the code into JavaScript/WebAssembly, and runs the cycle-based simulation in the browser.

The built-in examples demonstrate Verilog by emulating 1970s-era video games. The IDE displays a simulated CRT monitor, and allows control inputs from the keyboard and mouse. The example designs range from simple test patterns to CPU-driven video games.

The IDE is available online at https://8bitworkshop.com. The source code is at https://github.com/sehugg/8bitworkshop under a GPLv3 license. Sample code is CC0 unless indicated.

### Authors
1. Steven Hugg (8bitworkshop.com) <hugg@fasterlight.com>

# Article 16

## The Hardware Interchange Format
paper
[presentation](Videos/2022/16-Huang.mp4)
[slides](PDFs/2022/16-Huang.pdf)
[repo](https://github.com/masc-ucsc/hif)

### Abstract
There currently exists a plethora of open-source hardware design tools and compilers. There are also numerous open-source hardware designs written in different languages. We propose the Hardware Interchange Format (HIF), a file format to interchange circuits, netlists, and designs across various hardware design tools and compilers. In doing so, we propose a data format and an encoding to store data efficiently, allowing efficient interchange between different hardware design tools and compilers. We evaluate our results.

### Authors
1. Ramesh Jayaraman (University of California, Santa Cruz) <rkjayara@ucsc.edu>
2. Jing-Hsiang Huang (University of California, Santa Cruz) <jhuan278@ucsc.edu>
3. Jose Renau (University of California, Santa Cruz) <renau@ucsc.edu>

# Article 17

## PipelineC: Easy open-source hardware description between RTL and HLS
[paper](PDFs/2022/17-Kemmerer-poster.pdf)
[presentation](Videos/2022/17-Kemmerer.mp4)
[slides](PDFs/2022/17-Kemmerer-slides.pdf)
[repo](https://github.com/JulianKemmerer/PipelineC)

### Abstract
This poster session or short talk will describe the current status of the PipelineC project: https://github.com/JulianKemmerer/PipelineC.

Traditional hardware description languages (HDLs) like SystemVerilog and VHDL are notorious for their steep learning curves. High level synthesis (HLS) tools are also notorious for lack of precise hardware control and unexpected results. PipelineC aims to make hardware description easier for everyone from RTL designers to software minded HLS users.

The first step towards easier hardware description is a familiar, basic, C-like syntax. This makes ‘simulating in your head’ much easier than when reading any old RTL source file: where blocking and non-blocking assignments make combinatorial logic wiring/dataflow difficult to pull from the source RTL (let alone any simulation only constructs that can creep in). Instead in PipelineC simple C functions describing synthesizable feedforward dataflows are assumed.

Following the writing of any HDL, a designer must eventually face the task of timing analysis and meeting the required operating frequency for their design. Getting information on why paths are failing to meet timing is tool specific and often takes some effort to make sense of the post synthesis netlist/resource names. Instead, PipelineC works with many synthesis+PnR tools to give timing analysis information to the user with C function and variable names. This then makes it easier to make design changes that help fix problematic long timing paths.

However, there should be few surprising long timing paths because of PipelineC’s next feature: automatic pipelining of combinatorial logic. Using the timing information provided to the user, the tool internally automatically pipelines logic to a specified operating frequency (or fixed number of stages). Existing synthesis tools offer some small automatic pipelining when supplied with the proper registers for retiming. But PipelineC will auto-pipeline arbitrarily deep/wide chains of combinatorial logic: ex. hundreds of logic levels have been tested.

Several other advanced features can also be used to create complex designs: Point to point wires allow for composing designs in intuitive ways with easier syntax than traditional manual routing of wires through nested instantiated modules as in traditional HDL. Clock domain crossings are checked and have built in conversion between integer ratio streams of data. State machines can be derived from code that executes over several clock cycles, with familiar function call syntax for hierarchical design.

Finally, the tool renders human readable VHDL. This makes it easier to debug the HDL directly and supports all HDL synthesizers and simulators (VHDL->Verilog can be included, ex. for Verilator). Users can also insert arbitrary chunks of hand written VHDL, closing any gaps that exist when using PipelineC for full designs (ex. to wrap/instantiate existing IP cores).

Demos working in hardware include: Realtime raytraced retro style game, MNIST digit recognition neural network, cryptographic hashes, packet processing, I2S audio, AXI integration, and more.

PipelineC is in active development. Always happy to take questions, comments, suggestions on making the tool better.

### Authors
1. Julian Kemmerer (None) <julian.v.kemmere@gmail.com>

# Article 18

## IRSIM: A Switch-Level Simulator and Dynamic Power Analysis Tool
[paper](PDFs/2022/18-Liang-paper.pdf)
[presentation (long)](Videos/2022/18-Liang-long.mp4)
[presentation (short)](Videos/2022/18-Liang-short.mp4)
[slides](PDFs/2022/18-Liang.pdf)
[repo](https://github.com/RTimothyEdwards/irsim)

### Abstract
IRSIM is an open-source switch level simulator that analyzes digital circuits at the device (transistor) level using a linear switch-based model that depends on whether a transistor is "on" or "off" but accounting for the resistance through the device for delay estimates. This event-based simulation makes IRSIM much faster than a device modeling simulator like SPICE, but slower than a Verilog simulator, which models circuits at the gate level yet lacks a power analysis component. However, since Verilog simulations are still much faster than IRSIM for logic simulations, IRSIM has been largely ignored, and its dynamic power analysis feature forgotten. In this paper, we discuss the software methods in IRSIM with particular emphasis on further improving its dynamic power analysis capabilities.

### Authors
1. Jason Liang (UC San Diego) <jsliang@ucsd.edu>
2. R. Timothy Edwards (Efabless) <tim@efabless.com>

# Article 19

## Rapid Open Hardware Development Framework
[paper](PDFs/2022/19-Korbel-paper.pdf)
[presentation (long)](Videos/2022/19-Korbel-long.mp4)
[presentation (short)](Videos/2022/19-Korbel-short.mp4)
[slides](PDFs/2022/19-Korbel.pdf)
[repo](https://github.com/intel/rohd)

### Abstract
The Rapid Open Hardware Development (ROHD) framework is an open-source framework for describing and verifying hardware in the Dart programming language. ROHD enables engineers to build and traverse a graph of connectivity between module objects using unrestricted software. ROHD improves development iteration time by orders of magnitude and enables higher quality and more succinct designs, better abstraction through composition, and more powerful testbenches. It leverages modern software industry innovations like build, debug, profiling, and dependency management provided through the Dart ecosystem. ROHD includes a fast, event-based, four-value simulator with cosimulation support. Hardware models can be converted into logically equivalent, structurally similar, human readable, EDA tool compatible SystemVerilog with signal and port names maintained. ROHD can instantiate and interact with SystemVerilog modules, enabling gradual adoption of ROHD into derivative projects. The architecture of the framework is extensible to generate different kinds of output beyond just SystemVerilog. The ROHD Verification Framework, built upon ROHD, enables development of complex testbenches. ROHD aims to revolutionize hardware development and become a new industry standard.

### Authors
1. Max Korbel (Intel Corporation) <max.korbel@intel.com>

# Article 20

## A MLIR-Based Hardware Synthesis Framework
[paper](PDFs/2022/20-Xu-paper.pdf)
[presentation (long)](Videos/2022/20-Xu-long.mp4)
[presentation (short)](Videos/2022/20-Xu-short.mp4)
slides
repo

### Abstract
Hardware synthesis adopts a higher abstraction to improve the productivity of hardware design. High-level synthesis tools can automatically transform a high-level description into hardware design, while hardware generators adopt domain-specific languages and synthesis flows for specific applications. However, the implementation of these tools generally requires substantial engineering efforts due to RTL's weak expressivity and low level of abstraction. To lower the engineering cost and get competitive hardware design rapidly, we build Hector, a two-level IR providing a unified intermediate representation for hardware synthesis methodologies. The high-level IR binds computation with a control graph annotated with timing information, while the low-level IR provides a concise way to describe hardware modules and elastic interconnections among them. Implemented based on the multi-level compiler infrastructure (MLIR), Hector's IRs can be converted to synthesizable RTL designs. Different hardware synthesis approaches can adopt suitable levels of intermediate representations (IR) and are well supported in Hector with minimal engineering effort. The multi-level representation also enables optimizations like pipeline, which is hard to support at RTL.

### Authors
1. Ruifan Xu (Peking University) <xuruifan@pku.edu.cn>
2. Youwei Xiao (Peking University) <shallwe@pku.edu.cn>
3. Jin Luo (Peking University) <luo-jin@pku.edu.cn>
4. Yun Liang (Peking University) <ericlyun@pku.edu.cn>
