#  WOSET 2020 Proceedings

To cite an article, please use this format:   
(author names here), "(article title here)", Article No. (article number here), Workshop on Open-Source EDA Technology (WOSET), 2020.

For live discussions via Zoom and Slack, please see the [WOSET 2020 Schedule](WOSET2020-schedule.md).

# Article 1
## Hypergraph Partitioning via Geometric Embeddings

[paper](PDFs/2020/a01.pdf)
[presentation](https://www.youtube.com/watch?v=TMQremuD7SI&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=1)
[slides](PDFs/2020/a01-slides.pdf)
[repo](https://github.com/Breakinbad/Galois-1/tree/master/lonestar/experimental/embedding)

### Abstract
Hypergraph partitioning has been used in many
VLSI domains such as floor-planning, placement, and logic
synthesis. Circuits are modeled as hypergraphs in which nodes
represent the pins of the circuit and hyperedges represent nets
from the output pin of a gate to the input pins of other gates, and
the nodes are partitioned into a desired number of clusters so
that a metric such as the number of cut hyperedges is minimized.
Existing hypergraph partitioning techniques consider only the
topology of the hypergraph (connectivity between nodes) and
ignore its geometry (positions of nodes in 2D or 3D space). This
can lead to sub-optimal partitioning. In this paper, we describe
an embedding-based approach for hypergraph partitioning that
considers the geometry of circuits, which leads to better quality
partitions, while ensuring strong determinism.

### Authors
1. Sepideh Maleki <smaleki@cs.utexas.edu> (University of Texas at Austin)
2. Udit Agarwal <udit@utexas.edu> (UT Austin)
3. Keshav Pingali <pingali@cs.utexas.edu> (The University of Texas at Austin)

# Article 2
## Towards an Open-Source Verification Method with Chisel and Scala

[paper](PDFs/2020/a02.pdf)
[presentation](https://www.youtube.com/watch?v=5lwDoc2mbzE&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=2)
[slides](PDFs/2020/a02-slides.pdf)
[repo](https://github.com/chisel-uvm)

### Abstract
Performance increase with general-purpose processors has come to a halt.
We can no longer depend on Moore's Law to increase computing performance.
The only way to achieve higher performance or lower energy consumption
is by building domain-specific hardware accelerators.
To efficiently design and verify those domain-specific accelerators, we need
agile hardware development.

This paper presents a combination of open-source tools for verifying
circuits described in mixed languages. It builds on top of the Chisel
hardware construction language and uses Scala to drive the verification.
We also explore the testing strategy used in the Universal Verification Methodology
(UVM) in the context of verifying hardware described in Chisel.

### Authors
1. Martin Schoeberl <masca@dtu.dk> (Technical University of Denmark)
2. Simon Thye Andersen <simon.thye@gmail.com> (Technical University of Denmark)
3. Kasper Juul Hesse Rasmussen <s183735@student.dtu.dk> (Technical University of Denmark)
4. Richard Lin <richard.lin@berkeley.edu> (University of California, Berkeley)

# Article 3
## Google/SkyWater and the Promise of the Open PDK

[paper](PDFs/2020/a03.pdf)
[presentation](https://www.youtube.com/watch?v=nY6FVsAvrUo&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=3)
[slides](PDFs/2020/a03-slides.pdf)
[repo](http://github.com/google/skywater-pdk)

### Abstract
For over twenty years, silicon foundry Process Design Kits (PDKs) have been a domain of secret knowledge, non-disclosure agreements (NDAs), license servers, and password-protected download sites.  The lack of transparency is at odds with today's ever-expanding universe of open source software, leading to an unusual niche for licensed commercial tools, and a very difficult space in which to explore, grow, and diversify.  To overcome the problems inherent in this arrangement, the SkyWater foundry has opened up its process description to the public, a process driven and underwritten by Google and supported by efabless and a consortium of small companies and university groups.  This talk highlights the implications of having a free and publicly-accessible foundry process description on the small world of open source electronic design automation (EDA) tools for custom silicon design, how the open source PDK repository is beneficial to the worldwide chip design community, how developers of open-source EDA tools can take advantage of it, and where to move forward in a future of open-source tools and hardware.

### Author
Tim Edwards <tim@opencircuitdesign.com> (Open Circuit Design, efabless.com)


# Article 4
## A Push-button Idea to GDS-II SoC Design Flow

[paper](PDFs/2020/a04.pdf)
[presentation](https://www.youtube.com/watch?v=JaDumrEhuTU&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=4)
[slides](PDFs/2020/a04-slides.pdf)
[repo](https://github.com/habibagamal/SoC_Automation)

### Abstract
SoCGen is a system on chip (SoC) design automation
tool that takes in a simple JavaScript Object Notation (JSON)
description of the system’s components, connections and structure.
The tool then outputs the Verilog HDL for the SoC, the
intermediate files of hardening and the final GDS-II. SoCGen
utilizes OpenLANE, an automatic RTL to GDS-II physical design
flow. SoCGen is tailored for SoCs intended for internet of things
(IoT) and deep embedded applications.

### Authors
1. Habiba Gamal <habibabassem@aucegypt.edu> (The American University in Cairo)
2. Amr Gouhar <amrgouhar@aucegypt.edu> (eFabless)
3. Mohamed Shalan <mshalan@aucegypt.edu> (The American University in Cairo)


# Article 5
## CVC: Circuit Validity Checker An open source netlist reliabilty verification system

[paper](PDFs/2020/a05.pdf)
[presentation](https://www.youtube.com/watch?v=_JF2h35gFQ0&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=5)
[slides](PDFs/2020/a05-slides.pdf)
[repo](https://github.com/d-m-bailey/cvc)

### Abstract
This paper presents a device level static verification system for quickly and easily detecting common circuit errors in CDL (Circuit Definition Language) netlists. The system includes the capability to define device parameters and voltages for multiple modes in Microsoft Excel, an interactive option for examining intermediate values, and a GUI for analyzing the results. Errors detected are similar to those found using Mentor’s Calibre-PERC [1] or Synopsys’ CCK [2]. CVC has been used on dozens of DRAM and SOC designs of up to 3B devices.

### Author
Mitch Bailey <d.bailey@shuharisystem.com> (Shuhari System)


# Article 6
## An Open Source Alternative to Wire Bonding

[paper](PDFs/2020/a06.pdf)
[presentation](https://www.youtube.com/watch?v=-2M6OgjNXEw&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=6)
[repo](https://github.com/letter108/Wirebonding)

### Abstract
Before the end of the millennium, the infrastructure concerned with circuit chip design and development was widely accessible and affordable to many people involved; the relevant software was free and, and chips were cheap to manufacture. However, through the rapid development of electronics in the past twenty years, a vast majority of software and design tools became proprietary. The license costs for these became prohibitively expensive for all except large companies and research institutions, thus confining the chip design industry within the borders of privatized interests. Consequently, many university research programs, small companies, and individuals concerned with chip design have no choice but to work with obsolete technologies and methods. This paper discusses a recent initiative to 'democratize' the chip design industry through software automation. Specifically, we overview a desktop application that automates wire bonding chips to their respective packages, detail its functionality, and discuss the supporting infrastructure from which the application derives its resources from. We will also discuss any relevant and existing open source tools and the  shortcomings of the application.

### Authors
1. Pascal J Sossou <pascalsossou1@gmail.com> (Poolesville High School)
2. Tim Edwards <tim@opencircuitdesign.com> (Open Circuit Design, efabless.com)


# Article 7
## A power router for gridded cell placement

[paper](PDFs/2020/a07.pdf)
[presentation](https://www.youtube.com/watch?v=SNFo878h5OM&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=7)
[repo](https://github.com/asyncvlsi/PWRoute)

### Abstract
Electronic design automation (EDA) tools for asynchronous circuits, especially physical layout tools are limited. To improve  the  adoption  of  asynchronous  circuits,  Dali,  a  griddedcell placement flow was proposed. In the flow, the cell height and  width  can  be  any  integer  multiple  of  two  grid  values,  thus traditional  power  grid  generation  for  standard  cells  does  not apply and a dedicated power router is needed. In this work, we developed an open-source DRC-clean power router that supports the  gridded  placement  approach.  The  power  router  consists  of two  steps:  power  mesh  generation  and  detailed  power  routing. The  power  router  is  verified  by  commercial  tools  and  a  chiptape-out,  and  is  open-source  on  Github  [2]

### Authors
1. Jiayuan He <hejy@cs.utexas.edu> (University of Texas at Austin)
2. Yihang Yang <yihang.yang@yale.edu> (Yale University)
3. Rajit Manohar <rajit.manohar@yale.edu> (Yale University)


# Article 8
## A PostScript Toolkit for Electronic Design

[paper](PDFs/2020/a08.pdf)
[presentation](https://www.youtube.com/watch?v=G85pc5F1TBk&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=8)
[repo](https://github.com/profmadden/pstools)

### Abstract
Design automation tools operate on large problems, and often take hours or days to complete a run. Visualizing design data effectively can help track bugs, highlight optimization opportunies, and give a deeper understanding of the impact of subtle algorithmic changes. In this paper, we present a small, lightweight, cross-platform C language interface to the PostScript language, designed for software developers who primarily work in C or C++. Versions of this library have been a key resource for our research group in development of a number of design automation tools. The library is available in open source at https://github.com/profmadden/pstools.

### Authors
1. Sarp Ozdemir <sozdemi2@binghamton.edu> (SUNY Binghamton)
2. Jennifer Seibert <jseiber1@binghamton.edu> (SUNY Binghamton)
3. Mohammad A. Khasawneh <mkhasaw1@binghamton.edu> (SUNY Binghamton/MathWorks)
4. Patrick H. Madden <pmadden@binghamton.edu> (SUNY Binghamton)


# Article 9
## OpenPhySyn: An Open-Source Physical Synthesis Optimization Toolkit

[paper](PDFs/2020/a09.pdf)
[presentation](https://www.youtube.com/watch?v=Tx95__C4vFA&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=9)
[repo](https://github.com/scale-lab/OpenPhySyn)

### Abstract
Physical synthesis is a crucial phase in modern EDA design due to the challenges in achieving timing closure. Many approaches have been presented to solve different design problems and violations, such as buffer-insertion, gate-sizing, pin-swapping, gate-cloning, and logic transformations; each approach has different overhead costs in terms of area, power, and run-time. This paper describes OpenPhySyn, a new open-source EDA kit that implements and enhances different physical and logical design algorithms to resolve design violations and perform timing closure. The tool integrates seamlessly with standard EDA flows and tackles different types of violations with minimal human interference and reduced area overhead. Testing OpenPhySyn against different benchmarks with different characteristics from 46 violations up to 1200 violations showed that the tool solved most of the presented violations with only a 4\% average increase in the design area.

### Authors
1. Ahmed Agiza <ahmed_agiza@brown.edu> (Brown University)
2. Sherief Reda <sherief_reda@brown.edu> (Brown University)


# Article 10
## Universal Hardware Data Model

[paper](PDFs/2020/a10.pdf)
[presentation](https://www.youtube.com/watch?v=-L81ip8pkHg&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=10)
[slides](PDFs/2020/a10-slides.pdf)
[repo](https://github.com/alainmarcel/UHDM)

### Abstract
The Universal Hardware Data Model (UHDM) [1] Open source project aims at enabling Open source EDA tools to support the entire SystemVerilog 2017 Standard [2]. On one side parsers like Surelog [3] parse and populate the UHDM model and on the other side client tools like Synthesis, Simulation, Linters and so on read back from the compiled model and perform their tasks.
Keywords—SystemVerilog 2017, Open Source Parser, Persistent Data Model

### Authors
1. Alain Dargelas <alain.dargelas@gmail.com> (Data Model Solutions, LLC)
2. Henner Zeller <hzeller@google.com> (Google)


# Article 11
## Taskflow: A General-purpose Parallel and Heterogeneous Task Programming System for VLSI CAD

[paper](PDFs/2020/a11.pdf)
[presentation](https://www.youtube.com/watch?v=psQq-kG7nSs&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=11)
[repo](http://taskflow.github.io)

### Abstract
This paper introduces Taskflow to address the critical question of “How can we make it easier to implement and deploy parallel computer-aided design (CAD) algorithms on large heterogeneous nodes with high performance and simultaneous high productivity?” Parallelizing CAD is an extremely challenging job. Modern CAD applications exhibit unique computational patterns and user requirements that need very strategic decomposition to benefit from parallelism. Taskflow assists researchers and developers in the implementation complexity of parallel algorithms by introducing a new high-level programming model supported by an efficient run- time. By capitalizing on emerging parallelism comprising many- core central processing units (CPUs), graphics processing units (GPUs), and custom accelerators, Taskflow enables CAD to achieve new performance and productivity milestones that were previously out of reach.

### Authors
Tsung-Wei Huang <tsung-wei.huang@utah.edu>


# Article 12
## A Digital Flow for Asynchronous VLSI Systems: Status Update

[paper](PDFs/2020/a12.pdf)
[presentation](https://www.youtube.com/watch?v=wQEkFO0LaRw&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=12)
[slides](PDFs/2020/a12-slides.pdf)
[repo](https://github.com/asyncvlsi/)

### Abstract
We are developing an open-source EDA flow for asynchronous logic. Key parts of the flow are implemented using the Galois system for parallelization to reduce run-time requirements. We report on the current state of this flow, and some of the issues that we are exploring in order to improve the overall quality of results and expand the class of circuits that can be implemented using the flow.

### Authors
1. Udit Agarwal <udit@cs.utexas.edu> (University of Texas at Austin)
2. Samira Ataei <samira.ataei@yale.edu> (Yale University)
3. Jiayuan He <hejy@cs.utexas.edu> (University of Texas at Austin)
4. Wenmian Hua <wenmian.hua@yale.edu> (Yale University)
5. Yi-Shan Lu <yishanlu@cs.utexas.edu> (University of Texas at Austin)
6. Sepideh Maleki <smaleki@cs.utexas.edu> (University of Texas at Austin)
7. Yihang Yang <yihang.yang@yale.edu> (Yale University)
8. Keshav Pingali <pingali@cs.utexas.edu> (University of Texas at Austin)
9. Rajit Manohar <rajit.manohar@yale.edu> (Yale University)


# Article 13
## An Automatic Schematic Generation Tool for SPICE Netlists

[paper](PDFs/2020/a13.pdf)
[presentation](https://www.youtube.com/watch?v=_vJOEpMd3hM&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=13)
[slides](PDFs/2020/a13-slides.pdf)
[repo](https://github.com/aidangoettsch/asg)

### Abstract
This tool was designed and developed over this past summer to automatically create a schematic of a circuit given a SPICE representation. The algorithm implemented uses a series
of constraints which are applied iteratively to optimize a "score", which reflects how desirable a given arrangement of components and wires is. These constraints currently include a set of heuristics to determine optimal placements, as well as negative reinforcement for undesirable behaviors, such as crossing wires and intersecting components. The tool currently produces output for Xschem and KiCAD's EESchema. Xschem schematics include the necessary metadata for the Xschem netlist generator to produce a netlist which is identical to the original netlist. The main application of this tool is to create a schematic which represents a circuit which was created from a hardware description language. Since netlists produced from Xschem will be near identical to the input netlist, aside from any changes, this presents a workflow which allows for easy modifications to the netlist through manipulation of the generated schematic. This can be useful for fixing minor errors in circuits without needing to recompile the circuit, which could impact unrelated parts of the circuit, making it impossible to use already fabricated parts. Additionally, the codebase provides a generic interface for parsing SPICE and symbol libraries, as well as producing schematics, which alone can have applications outside of this particular problem. Future tasks include adding additional constraints and improving the behavior of existing ones, as well as optimizing the performance with large schematics.

Author
Aidan Goettsch <aidangoettsch@gmail.com> (Poolesville High School)


# Article 14
## Cocoon: An Open Source Infrastructure for Integrated EDA with Interoperability and Interactivity

[paper](PDFs/2020/a14.pdf)
[presentation](https://www.youtube.com/watch?v=CjUpLRRbWZw&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=14)
[slides](PDFs/2020/a14-slides.pdf)
[repo](https://github.com/pku-dasys/cocoon)

### Abstract
The increasing size and complexity of integrated circuit (IC) design introduce huge design cost and put forward higher requirements for EDA tools.
Improving the quality and efficiency of chip design requires the efforts of both EDA workers and IC designers.
In this paper, we first put forward the concept of Integrated EDA, a system composed of EDA points tools, designs and interfaces.
And we point out the key features of integrated EDA and the possible solutions.
Then we propose Cocoon, an open source infrastructure for integrated EDA with interoperability and interactivity.
It contains a set of cross-tool interfaces and plays the role of EDA agent that can help IC designers choose EDA point tools to assemble a legal design flow and to produce ICs with higher quality of results (QoR).
At last, we implement two demos using Cocoon to prove that such infrastructure is feasible and flexible for integrated EDA.

### Authors
1. Jiaxi Zhang <zhangjiaxi@pku.edu.cn> (Peking University)
2. Tuo Dai <daitoto@pku.edu.cn> (Peking University)
3. Zhengzheng Ma <alex_ma@pku.edu.cn> (Peking University)
4. Yibo Lin <yibolin@pku.edu.cn> (Peking University)
5. Guojie Luo <gluo@pku.edu.cn> (Peking University)


# Article 15
## PyVSC: SystemVerilog-Style Constraints, and Coverage in Python

[paper](PDFs/2020/a15.pdf)
[presentation](https://www.youtube.com/watch?v=JFKJSmP5Z3Q&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=15)
[slides](PDFs/2020/a15-slides.pdf)
[repo](https://github.com/fvutils/pyvsc)

### Abstract
Constrained-randomization and functional coverage are key elements in the widely-used SystemVerilog-based verification flow. The use of Python in functional verification is growing in popularity, but Python has historically lacked support for the constraint and coverage features provided by SystemVerilog. This paper describes PyVSC, a library that provides these features.

### Authors
Matthew Ballance <matt.ballance@gmail.com>


# Article 16
## Facilitating the Specification and Implementation of Pipelined Designs with Skeletor

[paper](PDFs/2020/a16.pdf)
[presentation](https://www.youtube.com/watch?v=rxc6PAnW_ak&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=16)
[repo](https://github.com/jaquerinte/Skeletor)

### Abstract
Skeletor is an open source EDA tool which reduces the bootstrap effort of new hardware designs. Skeletor facilitates the design specification as well as its automatic translation to the hierarchy of Verilog files, testbenches, synthesis and simulation scripts. In its 1.5 version we added support for the pipelined designs. In this paper, we describe the newly introduced feature and show its benefits with two real-world examples.

### Authors
1. Ivan Rodríguez <ivan.rodriguez@bsc.es> (Barcelona Supercomputing Center (BSC) and Universitat
   Politècnica de Catalunya (UPC))
2. Javier Barrera <javier.barrera@bsc.es> (Barcelona Supercomputing Center (BSC) and Universitat
   Politècnica de Catalunya (UPC))
3. Jeremy Giesen <jeremy.giesen@bsc.es> (Barcelona Supercomputing Center (BSC) and Universitat
   Politècnica de Catalunya (UPC))
4. Alvaro Jover <alvaro.jover@bsc.es> (Barcelona Supercomputing Center (BSC) and Universitat
   Politècnica de Catalunya (UPC))
5. Leonidas Kosmidis <leonidas.kosmidis@bsc.es> (Barcelona Supercomputing Center (BSC) and
   Universitat Politècnica de Catalunya (UPC))


# Article 17
## LSOracle: Using Mixed Logic Synthesis in an Open Source ASIC Design Flow

[paper](PDFs/2020/a17.pdf)
[presentation](https://www.youtube.com/watch?v=-MKlWXM1Gqw&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=17)
[repo](https://github.com/LNIS-Projects/LSOracle)

### Abstract
LSOracle is a free software logic synthesis tool that leverages
several types of underlying data structures and manipulation
methods, including And-Inverter Graphs and Majority-Inverter
Graphs to optimize highly heterogeneous circuit designs
automatically. It divides large designs at the module level and
selects the appropriate data structure and optimizer for each
module. It is available as a standalone tool, or as a Yosys
plugin, allowing easy integration with existing open source
EDA toolchains, and is capable of both ASIC and FPGA
synthesis. To demonstrate its capabilities, we present results
using LSOracle with the OpenROAD flow for ASIC synthesis,
targeting the BlackParrot benchmark and the Nangate45
library, both available in the OpenROAD repository. Using
LSOracle, delay is improved by up to 46% with negligible cost
in area and power. The tool is freely available at our GitHub
repository

### Authors
1. Scott Temple <scott.temple@utah.edu> (University of Utah)
2. Walter Lau Neto <walter.launeto@utah.edu> (University of Utah)
3. Max Austin <max.austin@utah.edu> (University of Utah)
4. Xifan Tang <xifan.tang@utah.edu> (University of Utah)
5. Pierre-Emmanuel Gaillardon <pierre-emmanuel.gaillardon@utah.edu> (University of Utah)


# Article 18
## An Open-source ToolSet for FPAA Design

[paper](PDFs/2020/a18.pdf)
[presentation](https://www.youtube.com/watch?v=s0eYW_kSWv4&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=18)
[repo](http://hasler.ece.gatech.edu/FPAAtool/index.html)

### Abstract
This open-source toolset enables targeting and design of the fine-grain SoC Large-scale Field Programmable Analog Array (FPAA)  family of devices, similar to tools enabling FPGA devices. The SoC  FPAA tool framework is presented, following a discussion of the resulting analog abstraction, FPAA infrastructure, and resulting educational and research  impact.

### Authors
1. Jennifer Hasler <jennifer.hasler@ece.gatech.edu> (Georgia Institute of Technology)
2. Aishwarya <anatarajan35@gatech.edu> (Natarajan)


# Article 19
## OpenFPGA: Towards Automated Prototyping for Versatile FPGAs

[paper](PDFs/2020/a19.pdf)
[presentation](https://www.youtube.com/watch?v=nwb5Yk5Uz5w&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=19)
[repo](https://github.com/LNIS-Projects/OpenFPGA)

### Abstract
This paper introduces an open-source framework
OpenFPGA which aims to automate the design, verification
and layout of highly versatile FPGA architectures. OpenFPGA
offers a high-level architecture description language for users
to customize their FPGA architectures down to circuit-level
details. Based on the architecture modeling, OpenFPGA can
auto-generate Verilog netlists, with which users can perform
verification as well as generate production-ready layouts using
modern EDA tools. OpenFPGA includes a generic Verilog-to-
Bitstream generator, as a native EDA toolchain for any FPGAs
that are prototyped by OpenFPGA. To demonstrate the capability
of OpenFPGA, we showcase the <24-hour layout generation of
two FPGA fabrics which are based on Stratix-like architecture
built with a commercial 12nm standard-cell library and 40nm
custom cells respectively.

### Authors
1. Xifan Tang <xifan.tang@utah.edu> (University of Utah)
2. Ganesh Gore <ganesh.gore@utah.edu> (University of Utah)
3. Edouard Giacomin <edouard.giacomin@utah.edu> (University of Utah)
4. Aur´elien Alacchi <aurelien.alacchi@utah.edu> (University of Utah)
5. Baudouin Chauviere <baudouin.chauviere@utah.edu> (University of Utah)
6. Pierre-Emmanuel Gaillardon <pierre-emmanuel.gaillardon@utah.edu> (University of Utah)


# Article 20
## Edalize it. Don’t critizise it

[paper](PDFs/2020/a20.pdf)
[presentation](https://www.youtube.com/watch?v=HuRtkpZqB34&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=20)
[repo](https://github.com/olofk/edalize)

### Abstract
Edalize (https://github.com/olofk/edalize) is an abstraction library for interfacing different EDA tools with a single description of the input files and tool configuration.

### Authors
Olof Kindgren <olof.kindgren@gmail.com> (FOSSi Foundation, Qamcom)


# Article 21
## OpenLANE: The Open-Source Digital ASIC Implementation Flow

[paper](PDFs/2020/a21.pdf)
[presentation](https://www.youtube.com/watch?v=bCwjb3l7oY4&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=21)
[slides](PDFs/2020/a21-slides.pdf)
[repo](https://github.com/efabless/openlane)

### Abstract
OpenLANE is a tape-out-hardened flow that addresses
two main use cases: hardening a macro and integrating
a System-on-a-Chip (SoC). It was used successfully to tape out
a family of RISC-V based SoCs known as “striVe”. This paper
reviews the various components of the flow with a particular focus
on the challenges that faced SoC integration while working on
the first of the striVe chips and the main ideas used to overcome
them, achieving full automation.

### Authors
1. Ahmed Ghazy <ax3ghazy@aucegypt.edu> (eFabless)
2. Mohamed Shalan <mshalan@aucegypt.edu> (The American University in Cairo)


# Article 22
## Pillars: An Integrated CGRA Design Framework

[paper](PDFs/2020/a22.pdf)
[presentation](https://www.youtube.com/watch?v=oNLyD6koB2g&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=22)
[slides](PDFs/2020/a22-slides.pdf)
[repo](https://github.com/pku-dasys/pillars)

### Abstract
In this paper, we propose Pillars, an integrated CGRA design framework, to assist in design space exploration and hardware optimization of CGRA.
Pillars allows an architect to describe a hierarchical CGRA design in a Scala-based language and produce an in-memory model for both behavior and structure.
The model generates the RTL code and the structure for reconfiguration.
This structure enables application mapping and context generation in a flattened representation generated from a hierarchical model.
Thus, CAD tools in Pillars are able to map applications onto the architecture and produce contexts that enable cycle-accurate simulations.
In the experimental evaluation, we demonstrate the capability of Pillars to model CGRA architectures by synthesizing variants of a widely known CGRA architecture, ADRES, into FPGA overlays.


### Authors
1. Yijiang Guo <yijiang@pku.edu.cn> (Peking University)
2. Guojie Luo <gluo@pku.edu.cn> (Peking University)


# Article 23
## Automatically Building Digital Symbol Libraries

[paper](PDFs/2020/a23.pdf)
[presentation](https://www.youtube.com/watch?v=21oHjfWXpPY&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=23)
[repo](https://github.com/arjunr10/eda-symbol_libraries)

### Abstract
Digital circuit symbols do not currently have commonly accepted open standards for the formats of such symbols. Consequently, digital cell libraries often come in proprietary formats. The purpose of this project is to automatically create a digital symbol library from a liberty file in the SkyWater pdk. An algorithm was developed in Python and a standard digital cell library was created in KiCad and XSCHEM. The algorithm is able to parse through the liberty file, store information on the cells, and successfully output a digital symbol library. In future work, steps will be taken to automatically create a spice netlist from the liberty file.
Git Hub repository: https://github.com/arjunr10/eda-symbol_libraries

### Authors
Arjun Rakheja <arjun.rakheja@gmail.com> (Poolesville High School in Montgomery County, MD.)


# Article 24
## AxLS: An Open-Source Framework for Netlist Transformation Approximate Logic Synthesis

[paper](PDFs/2020/a24.pdf)
[presentation](https://www.youtube.com/watch?v=CasrIWmbIZ4&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=24)
[slides](PDFs/2020/a24-slides.pdf)
[repo](https://github.com/ECASLab/AxLS)

### Abstract
With the rise of Approximate Computing as an energy-efficient design paradigm for error-tolerant applications, different Approximate Logic Synthesis (ALS) approaches have been proposed to generate approximate circuits from accurate implementations automatically. In this paper, we present AxLS, our open-source framework for ALS techniques based on structural netlist transformations. We describe our framework and provide an experimental evaluation for arithmetic circuits with our current implementation. AxLS enables the study and test of existing ALS techniques based on netlist transformations and the proposition of new ones, and it is available to download at https://github.com/ECASLab/AxLS.

### Authors
1. Jorge Castro-Godínez <jorge.castro-godinez@kit.edu> (Karlsruhe Institute of Technology)
2. Humberto Barrantes-García <mabaga1501@gmail.com> (Instituto Tecnológico de Costa Rica)
3. Muhammad Shafique <muhammad.shafique@nyu.edu> (New York University Abu Dhabi)
4. Jörg Henkel <henkel@kit.edu> (Karlsruhe Institute of Technology)


# Article 25
## GOLDMINE: A tool for enhancing verification productivity

[paper](PDFs/2020/a25.pdf)
[presentation](https://www.youtube.com/watch?v=MdQY2NGfZtI&list=PLItVYhgea-kEV15gg-D_rm7VG8bg20_XV&index=25)
[repo](https://sites.google.com/view/goldmine-illinois/home)

### Abstract
We present GOLDMINE, an efficient, modular, scalable, open-source tool with a set of rich features targeting a wide spectrum of hardware design analysis. GOLDMINE uses multiple technologies as part of its design analysis at the Register Transfer Level (RTL). In this work, we leverage different features for various hardware verification use cases such as design understanding, assertion generation,  debugging and bug localization,  assertion ranking,  and coverage analysis.

### Authors
1. Debjit Pal <work.debjitpal@gmail.com> (University of Illinois at Urbana-Champaign)
2. Vibhor Dodeja <vdodeja2@illinois.edu> (University of Illinois at Urbana-Champaign)
3. Anjana S. Kumar <anjanas3@illinois.edu> (University of Illinois at Urbana-Champaign)
4. Shobha Vasudevan <shobhav@illinois.edu> (University of Illinois at Urbana-Champaign)


