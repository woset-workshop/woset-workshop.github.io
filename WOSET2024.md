#  WOSET 2024 Proceedings

To cite an article, please use this format:
(author names here), "(article title here)", Article No. (article number here), Workshop on Open-Source EDA Technology (WOSET), 2024.

For live discussions via Zoom and Slack, please see the [WOSET 2024 Schedule](WOSET2024-schedule.md).

## Organization

### Co-Chairs
* Jose Renau, UC Santa Cruz (Co-Chair)
* Matthew Guthaus, UC Santa Cruz (Co-Chair)

### Program Chair
* Dustin Richmond, UC Santa Cruz

### Proceedings Chair
* Dan Petrisko, University of Washington

### Zoom Czar
* Haoyuan Wang, UC Santa Cruz

### Program Committee
* Jonathan Balkind, UC Santa Barbara
* Tim Edwards, efabless
* Steve Hoover, Redwood EDA
* Lucas Klemmer, JKU Linz
* Dirk Koch, University of Manchester
* Christian Krieg, TU Wien
* Rajit Manohar, Yale University
* Guillem Lopez Paradis, Barcelona Supercomputing Center
* Frans Skarman, Linköping University
* Matt Venn, YosysHQ, TinyTapeout

# Article 7

## Scaling Program Synthesis Based Technology Mapping with Equality Saturation
[paper](PDFs/2024/7_Scaling_Program_Synthesis_Ba.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
State-of-the-art hardware compilers for FPGAs often fail to find efficient mappings of high-level designs to low-level primitives, especially complex programmable primitives like digital signal processors (DSPs). New approaches apply sketch-guided program synthesis to more optimally map designs. However, this approach has two primary drawbacks. First, sketch-guided program synthesis requires the user to provide sketches, which are challenging to write and require domain expertise. Second, the open-source SMT solvers which power sketch-guided program synthesis struggle with the sorts of operations common in hardware—namely multiplication. In this paper, we address both of these challenges using an equality saturation (eqsat) framework. By combining eqsat and an existing state-of-the-art program-synthesis-based tool, we produce Churchroad, a technology mapper which handles larger and more complex designs than the program-synthesis-based tool alone, while eliminating the need for a user to provide sketches.

### Authors
1. Gus Henry Smith <gussmith@cs.washington.edu>
2. Colin Knizek <knizek@berkeley.edu>
3. Daniel Petrisko <petrisko@cs.washington.edu>
4. Zachary Tatlock <ztatlock@cs.washington.edu>
5. Jonathan Balkind <jbalkind@ucsb.edu>
6. Gilbert Louis Bernstein <gilbo@cs.washington.edu>
7. Haobin Ni <hn42@cs.washington.edu>
8. Chandrakana Nandi <cnandi@cs.washington.edu>

# Article 14

## Hardware and software build flow with SoCMake
[paper](PDFs/2024/14_Hardware_and_software_build.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
With the growing demand for electronics and the increasing complexity of system-on-chip (SoC) designs, there is a pressing need for efficient build systems that can handle both hardware and software components. This paper presents SoCMake, an innovative build system designed to streamline the development of SoC designs by integrating hardware and software build flows. Leveraging the robust CMake ecosystem, SoCMake offers essential features such as IP block abstraction, support for electronic design automation (EDA) tools, and effective package management. The proposed system aims to enhance build automation in hardware design, reduce complexity, and improve efficiency. A stable core API version 1.0.0 is scheduled for release by the end of 2024, with plans to broaden EDA tool support to compete with existing build systems.

### Authors
1. Risto Pejašinović <risto.pejasinovic@gmail.com>
2. Alessandro Caratelli <alessandro.caratelli@cern.ch>
3. Anvesh Nookala <anvesh.nookala@cern.ch>
4. Benoît Walter Denkinger <benoit.denkinger@cern.ch>
5. Marco Andorno <marco.andorno@cern.ch>

# Article 4

## pyngspice: A High-performance Python Binding for Ngspice
[paper](PDFs/2024/4_pyngspice_A_High_performance.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
This paper introduces pyngspice, a Python binding for ngspice that overcomes the performance limitations of existing solutions. Implemented as a Python C extension, pyngspice achieves near-native execution speeds while integrating seamlessly with Python’s ecosystem, including libraries such as NumPy and pandas. Benchmarks show significant improvements, with pyngspice reducing simulation time by approximately 50% for simple circuits compared to PySpice, and reducing overall training time in reinforcement learning applications by more than 20%, and nearly 50% compared to the ngspice executable method. These results highlight the effectiveness of the pyngspice framework for time-sensitive simulations and its potential to bridge the gap between high-performance circuit simulations and modern data-driven workflows.
 
### Authors
1. Jihyeon Park <falon18@hanyang.ac.kr>
2. Mintae Kim <alsxo326@hanyang.ac.kr>
3. Jaeduk Han <jdhan@hanyang.ac.kr>

# Article 9

## The Educational RISC-V Microprocessor Wildcat
[paper](PDFs/2024/9_The_Educational_RISC_V_Micro.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
Today, in teaching computer architecture, we use the RISC-V instruction set to explain the basics of a microprocessor. Initially, we introduce a conceptual single-cycle implementation of a RISC-V microprocessor, followed by a detailed presentation of a pipelined implementation of RISC-V. We can support this topic in teaching with executable implementations of RISC-V.
This paper presents two implementations of the RISC-V instruction set architecture: (1) an instruction set simulator to explore the RISC-V instructions set and (2) a pipelined implementation of RISC-V. We name this processor Wildcat, after a nice hiking area close to where RISC-V was developed, at the University of California, Berkeley. Wildcat is available under the BSD 2-Clause License at https://github.com/schoeberl/wildcat

### Authors
1. Martin Schoeberl <masca@dtu.dk>

# Article 12

## YoYoLint – a custom SystemVerilog RTL linter for Yosys
[paper](PDFs/2024/12_YoYoLint_a_custom_SystemVer.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
YoYoLint is an open-source static analysis tool designed for SystemVerilog RTL code. Written in Python and built around Slang/PySlang YoYoLint derives learnings from PySlint, a popular SystemVerilog testbench linter. YoYoLint aims to assist users in ensuring their SystemVerilog code is well-prepared for synthesis with Yosys, a popular, opensource RTL synthesis tool. YoYoLint helps users prepare SystemVerilog code for synthesis with Yosys, an open-source RTL synthesis tool. It provides a set of configurable linting rules that focus on detecting code patterns and issues that might cause problems during synthesis with Yosys.
The tool runs efficiently and delivers clear feedback on code violations. Users can run YoYoLint before synthesis with Yosys to find and fix issues, improving code quality and compatibility. YoYoLint is extendable, allowing users to add custom linting rules. It is regularly updated by analyzing SystemVerilog designs with Yosys, incorporating new unsupported features into its rule set. This ensures YoYoLint remains useful for current coding practices. The paper also addresses the role of linters in managing coding styles and avoiding common pitfalls in SystemVerilog. It provides an overview of YoYoLint’s development, potential extensions, and initial results. We share our experience in building YoYoLint and potential extensions. We conclude with the results on a few early use cases.

### Authors
1. Ajeetha Kumari Venkatesan <ajeethak@asfigo.com>
2. Deepa Palaniappan <deepa@asfigo.com>
3. Saanvi Pradhan <saanvi.pradhan@gmail.com>

# Article 2

## eSim: An Open-Source EDA Tool for Education
[paper](PDFS/2024/2_eSim_An_Open_Source_EDA_Tool.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
eSim is an open-source Electronic Design Automa- tion (EDA) tool designed for circuit design, simulation, and analysis [1]. Developed with a focus on providing an accessible and cost-effective solution for engineers, students, and hobbyists, eSim integrates various open-source tools to offer a comprehen- sive platform for analog and digital circuit design. This paper explores the major capabilities of eSim, its workflow for analog and digital design, [2] and presents case studies demonstrates its practical applications. Along with its capabilities, there are free audio-video tutorials available called Spoken Tutorials [6] through which the users can learn the software very easily

### Authors
1. Varad Patil <varadpatilofficial@gmail.com>
2. Roshan Binu Paul <roshanbinu2002@gmail.com>
3. Sumanto Kar <sumantokar@iitb.ac.in>
4. Kannan M. Moudgalya <kannan@iitb.ac.in>

# Article 5

## Status overview of the IHP OpenPDK Initiative: Technology - Devices - IC Designs
[paper](PDFs/2024/5_Status_overview_of_the_IHP_O.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
The semiconductor industry has undergone dynamic evolution and innovation for the past 75 years since the invention of the first semiconductor transistor. This rapid growth is driven by the direct and proactive contribution of the FOSS CAD/EDA to the entire technology flow: from state-of-the-art semiconductor technologies, device level compact/SPICE modeling, its Verilog-A standardization to advanced IC designs for various HiTech applications. However, the semiconductor industry also faces many challenges in maintaining the growth of its workforce with skilled technicians and engineers. To address the increasing need for well-trained workers worldwide, we must find innovative ways to attract skilled talent and strengthen the local semiconductor workforce ecosystem. The FOSS CAD/EDA tools with the recently available open access PDKs provide a new platform to connect IC design beginners, enthusiasts and experienced mentors to benefit from the collaboration opportunities enabled by the fast-growing open-source IC design movement. The collaborative development of open-source integrated circuit (IC) designs is becoming increasingly feasible due to the rapid expansion of OpenPDKs recently offered by SkyWater, GF and IHP with an open schedule of MPW Runs for FMD-QNC project in 2024-25. This paper demonstrates the FOSS CAD/EDA contribution to the SPICE/Verilog-A modeling/standardization, compete IC design flow (Xschem, Qucs-S, ngspice, Xyce, OpenVAF, OpenEMS, Magic, kLayout, OpenRoad), in addition selected, open-source examples of analog/RF and digital IC designs will be presented.

### Authors
1. Wladek Grabinski (presenter)
2. Rene Scholz
3. Sergei Andreev
4. Christian Wittke
5. Frank Vater
6. Norbert Herfurth
7. Krzysztof Herman
8. Sebastien Martinie
9. Matthias Bucher
10. Mike Brinson
11. Mustafa Alchalabi
12. Jan T aro Svejda
13. Christoph Sandner
14. Harald Pretl
15. Frank K. Gurkaynak

# Article 15

## Lighter: An Open-Source Automatic Clock Gating tool for Dynamic Power Reduction in ASIC
[paper](PDFs/2024/15_Lighter_An_Open_Source_Auto.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
This paper introduces Lighter, an automatic register clock gating utility designed to primarily reduce dynamic power, and reduce the area of gate-level designs as a subsidiary objective. Lighter specifically focuses on enabling automatic clock gating for load-enabled registers by providing a Yosys plugin and complementary technology mapping files. The current version of Lighter offers support for both the open-source Sky130 and GF180mcu standard cell libraries, and future versions aim to expand compatibility to include other libraries of other open-source Process Design Kits (PDKs). Through extensive experimentation, Lighter has demonstrated remarkable power and area reduction. The maximum power reduction achieved is 43.00%, while area reductions reached up to 58.21%. These results highlight Lighter’s significant potential in enhancing efficiency and optimizing resource utilization in digital circuit design.

### Authors
1. Youssef Kandil <youssefkandil@aucegypt.edu>
2. Mohamed Shalan <mshalan@aucegypt.edu>

# Article 11

## ORAssistant: A Custom RAG-based Conversational Assistant for OpenROAD
[paper](PDFs/2024/11_ORAssistant_A_Custom_RAG_ba.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
Open-source Electronic Design Automation (EDA) tools are rapidly transforming chip design by addressing key barriers of commercial EDA tools such as complexity, costs, and access. Recent advancements in Large Language Models (LLMs) have further enhanced efficiency in chip design by providing user assistance across a range of tasks like setup, decision-making, and flow automation. This paper introduces ORAssistant, a conversational assistant for OpenROAD, based on Retrieval-Augmented Generation (RAG). ORAssistant aims to improve the user experience for the OpenROAD flow, from RTL-GDSII by providing context-specific responses to common user queries, including installation, command usage, flow setup, and execution, in prose format. Currently, ORAssistant integrates OpenROAD, OpenROAD-flow-scripts, Yosys, OpenSTA, and KLayout. The data model is built from publicly available documentation and GitHub resources. The proposed architecture is scalable, supporting extensions to other open-source tools, operating modes, and LLM models. We use Google Gemini as the base LLM model to build and test ORAssistant. Early evaluation results of the RAG-based model show notable improvements in performance and accuracy compared to non-fine-tuned LLMs.

### Authors
1. Aviral Kaintura <102ctbmti2122019@nfsu.ac.in>
2. Palaniappan R <f20212915@hyderabad.bits-pilani.ac.in>
3. Shui Song Luar <jluar@precisioninno.com>
4. Indira Iyer Almeida <iiyer@precisioninno.com>

# Article 17

## OpenLane 2: Making the Most Popular Open Source ASIC Flow Modular
[paper](PDFs/2024/17_OpenLane_2_Making_the_Most_.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
We present OpenLane 2, a re-imagining of the world's most popular open-source RTL-to-GDSII flow as a modular infrastructure for flow creation. We show how the infrastructure has been architected to make flows more flexible, and crucially, repeatable. We demonstrate how we enhanced the flow's distribution and delivery using the Nix build and deployment system. Finally, we show some of the active current uses of OpenLane 2 in industry and academia.

### Authors
1. Mohamed Gaber <donn@efabless.com>
2. Kareem Farid <kareem.farid@efabless.com>
3. Bassant Hassan <bassant.hassan@efabless.com>
4. Mohamed Shalan <mshalan@aucegypt.edu>

# Article 18

## Simulating a Million-Core System with Switchboard
[paper](PDFs/2024/18_Switchboard.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
Immense hardware systems are needed to train state-of-the-art machine learning applications such as large language models. The design process for such hardware requires simulation for both architectural exploration and design verification; this can be challenging with traditional simulation approaches due to long build and run times. In this paper, we show how to make simulation tractable for large hardware systems with Switchboard, our open-source modular simulation framework. Switchboard facilitates scalable simulation by connecting prebuilt simulators of reasonably-sized hardware blocks through high-performance shared-memory queues. Each queue conveys a latency-insensitive interface, eliminating the need for explicit synchronization, which can otherwise hamper performance. Using Switchboard, we successfully performed an RTL simulation of a million-core system on thousands of cloud compute cores. The total time to build the design and simulate a distributed matrix multiplication was under 15 minutes, demonstrating the agility of our approach.

### Authors
1. Steven Herbst
2. Noah Moroze
3. Edgar Iglesias
4. Andreas Olofsson

# Article 3

## A Fast, Accurate, and Open-Source Simulation Tool for High-Level Synthesis
[paper](PDFs/2024/3_A_Fast_Accurate_and_Open_Sou.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
High-level synthesis (HLS) tools enable developers to write software code in C, C++, or SystemC and generate hardware RTL code in Verilog or VHDL, making it easier to develop complex hardware designs. However, to evaluate these designs, developers typically still rely on slow RTL simulators that can take hours to provide feedback, especially for complex designs. We introduce LightningSim, an open-source simulation tool for HLS designs that produces “RTL-like” latency estimates with “C-like” speed. LightningSim directly operates on the LLVM intermediate representation (IR) code of an HLS design and accurately simulates a hardware design's dynamic behavior. First, it traces LLVM IR execution to capture the run-time information; second, it maps the static HLS scheduling information to the trace to simulate the dynamic behavior; third, it calculates stalls and deadlocks from inter-function interactions to get precise cycle counts. Evaluated on 33 benchmarks, LightningSim produces 99.9%-accurate timing estimates up to 146× faster than RTL simulation. Our code and benchmark scripts, written in a combination of Python and Rust, are open-source on GitHub, licensed under the AGPL-3.0 license, and were awarded badges for artifact reproducibility.

### Authors
1. Rishov Sarkar <rishov.sarkar@gatech.edu>
2. Cong (Callie) Hao <callie.hao@ece.gatech.edu>

# Article 8

## Integrating Asynchronous Circuits into the Caravel Testing Harness
[paper](PDFs/2024/8_Integrating_Asynchronous_Cir.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
The Caravel harness has been widely used to tape-out synchronous designs in the open-source SKY130 PDK. To use this flow for asynchronous circuit design using the open-source Act framework, we can treat Act-generated layout as an asynchronous macro. We develop an open-source toolflow that supports this approach. This paper presents the challenges encountered during the integration of an asynchronous macro in the Caravel harness and the methods employed to address these issues, including power ring generation and connection, pin extension, and custom fill insertion. In addition, we discuss the process of transferring data to the asynchronous circuit using Caravel’s utilities.

### Authors
1. Thomas Jagielski <thomas.jagielski@yale.edu>
2. Xiayuan Wen <xiayuan.wen@yale.edu>
3. Matthew Dobre <matthew.dobre@yale.edu>
4. Rajit Manohar <rajit.manohar@yale.edu>

# Article 13

## An RFIC-oriented flow for Planar Inductors modeling and generation aiming Open-Source PDKs
[paper](PDFs/2024/13_An_RFIC_oriented_flow_for_P.pdf)
[presentation(long)]()
[presentation(short)]()
[slides]()
[repo]()

### Abstract
This paper presents an RFIC-oriented flow that aims to provide a way to modeling and generation of inductors based on open-source PDKs. A proposed flow is presented in order to be part of an RFIC design flow compatible with mainstream Analog open source development. An LC filter example using skywater 130 nanometer open-PDK is provided to show the proposed flow and its integration with other open-source tools that aim to obtain a final verified RFIC layout.

### Authors
1. Hugo Dias Gilo <hugo.gilo@alunos.ufersa.edu.br>
2. Francisco Brito-Filho <francisco.brito@ufersa.edu.br>
