#Project Title: Newer Nonvolatile Solid-State Memory Technology
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Team members/position:
-
	Leader: Aquino, Shannon Dale
	Rapporteur: Casalme, Christian
		    Gucilatar, Narold Jayson

Brief Description:

	Nonvolatile memory is a type of memory that can retain data even when power is turned off. Typically, it is used as secondary storage and long-term storage. Examples of Nonvolatile memory are computer hard disks and flash drives. Only when reading and writing data does it require power. Nonvolatile memory is perfect for long retention of information.
	Considering the many advantages of using Nonvolatile memory, it is inevitable for the demand to increase in the coming years. In this research project we shall discuss emerging Nonvolatile Solid-state Technologies that are currently being used. 


Table of Contents
-
	STT-RAM
	- Architecture
	- Application

	PCRAM
	- Architecture
	- Hybrid Technology of PCRAM
		- PCM and STT-RAM Hybrid
		- PCRAM and DRAM Hybrid
	- Application

	ReRAM
	- Architecture
	- Types of ReRAM
		- OxRAM
		- CBRAM
	- Application



PHASE 3: Project Documentation

Project Title: Newer Nonvolatile Solid-State Memory Technology 

Team Members:
	
	Aquino, Shannon Dale 
	Casalme, Christian
	Gucilatar, Narold Jayson

Abstract:

	Nonvolatile memory is a type of memory that can retain data even when power is turned off. Typically, it is used as secondary storage and long-term storage. Examples of Nonvolatile memory are computer hard disks and flash drives. Only when reading and writing data does it require power. Nonvolatile memory is perfect for long retention of information.
	
	Considering the many advantages of using Nonvolatile memory, it is inevitable for the demand to increase in the coming years. In this research project we shall discuss emerging Nonvolatile Solid-state Technologies that are currently being used. In line with the Computer Architecture and Organization 10th Edition we shall only be discussing STT-RAM, PCRAM and ReRAM. Through this project we shall give a detailed description about these said topics


STT-RAM

Architecture & Application

	STT stands for Spin-Transfer Torque. In an STT-RAM device, the spin of the electrons is flipped using a spin-polarized current. This effect is achieved in a magnetic tunnel junction (MTJ) or a spin-valve, and STT-RAM devices use STT tunnel junctions (STT-MTJ). A spin-polarized current is created by passing a current through a thin magnetic layer. This current is then directed into a thinner magnetic layer which transfers the angular momentum to the thin layer which changes its spin.

	STT-RAM has the potential to become a leading storage technology as it is a high-performance memory that can scale well below 10nm and challenge the low cost of flash memory. The main advantage of STT-RAM is the ability to scale the STT-RAM chips to achieve higher densities at a lower cost.

	As a discrete memory device, STT-MRAM is being used as a replacement for SRAM, DRAM, and NOR-flash due to its higher speed, lower latency, scalability, and unlimited endurance. STT-MRAM does not require a power-refresh like DRAM, and the read process is not destructive. This situation provides a significant power advantage, as well as lower latency at the system level.



PCRAM

Architecture

	Phase change memory(pcram) is a type of memory that stores data by altering the state of matter from which the device is fabricated. It can exist in two states amorphous and crystalline phases. These are reversible structural phrases. PCRAM, also known as PCM has fast read access time, good data retention and high data density. Several major memory manufacturers like Samsung, micron have already made a prototype with the implementation of PCM memory implementation.

	The architecture of PCM has a phase changing material and a narrow electrode called the heater. Between the two electrodes, chalcogenide is commonly used phase changing material. When Chalcogenide is heated and cooled slowly, it retains its amorphous state. In this state, it is highly resistive. This state represents the logic zero. When it is heated and cooled rapidly it becomes crystalline. In this state, it is less resistive and this state represents the logic 1. Write operation is performed by SET or RESET to write the logical 1 or 0 to the memory cell.

Hybrid Technology of PCRAM

PCM and STT-RAM Hybrid

	The hybrid technology is made possible with the spin torque transfer ram and the PCM. The small capacity of STT-RAM is used as a WRITE buffer with a PCM based cache. This Hybrid cache reduces the endurance limitation of PRAM cache by redirecting the WRITE traffic from an upper memory layer to the spin torque transfer ram WRITE buffer. The STT-RAM has virtually no WRITE limitation. However, the STT-RAM has a lower density than PCRAM. So, from the combination of the advantages of these two RAM benefits each other.  The high WRITE endurance of STT-RAM and the high density of PRAM  together increases the lifetime of PCRAM by redirecting the WRITE traffic towards STT-RAM. The technique used is that when there is a data to be written to the PCM, the new data is complied with the old data and the WRITE is triggered when the content of the cells are not matching. This was further improved by using an inverse bit, so if the number of bits to be written is more than half, the WRITE is triggered after inversing the data to be written.
	
PCRAM and DRAM Hybrid

	Another hybrid architecture that uses a small amount of DRAM together with PRAM makes an efficient memory.  This hybrid technology has been widely accepted. While PRAM consumes low READ and Sand by power DRAM consumes low WRITE power and provide WRITE endurance. The challenge in design is that the wear leveling of PRAM pages must be managed efficiently to ensure it’s longer lifetime. The hardware part is in the memory controller and manages the access information to different PRAM pages. The software portion is the part of the operating system “the memory manager”  which reduces the wear leveling by page swapping. The memory controller is aware of the partitioning of the system memory between PRAM and DRAM. Based on the accessed address, it is able to route a request to the correct memory. The memory controller keeps the map of a number of WRITE access to it. This information is maintained and when the numbers of WRITE accessed the given threshold to any PRAM page then the controller triggers a page swap interrupt to the processor and issues the page address. The operating system then uses the page manager to perform the page swap operations.



ReRAM

Architecture

	Resistive Random Access Memory is a new type of memory designed to be an alternative non-volatile memory (NVM) solution, particularly in cloud and data center environments which requires ever-increasing improvements in performance and energy efficiency. The ReRAM works by changing the resistance across a dielectric solid-state material, often referred to as a memristor.

	The principal advantage of RRAM over other non-volatile technology is high switching speed. Because of the thinness of the memresistors, it has a great potential for high storage density, greater read and write speeds, lower power usage, and cheaper cost than flash memory. Flash memory cannot continue to scale because of the limits of the materials, so RRAM will soon replace flash memory.

	Most ReRAM cells are made up of switching materials with various resistance characteristics sandwiched between two metallic electrodes. The switching effect of ReRAM is based on the motion of ions under the influence of an electrical field and the switching material’s ability to store the ion distribution. In turn, this causes a measurable change in the resistance of ReRAM devices, reducing the effects of dielectric breakdown that degrades memory component performance over time.

Types of ReRAM

OxRAM

	In OxRAM, a metal oxide material is sandwiched between the two electrodes. When a positive voltage is applied on the top electrode, a conductive filament forms between the two electrodes. The filament consists of ion atoms.

	When a negative voltage is applied on the bottom electrode, the conductive filament breaks. In effect, ReRAM switches between high and low resistive states. The change in resistance is represented by “0” and “1” in the memory.

CBRAM

	Like OxRAM, CBRAM also builds and destroys the filament to create resistive states. In CBRAM, though, a copper or silver metal is injected into the silicon, which forms a conductive bridge or filament between the two electrodes.

	Others are working on a non-filamentary approach. Instead of forming a filament, this technology uses a self-rectifying technique to form a switching effect. Some classify this technology as an OxRAM.



Reference:
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
	• Shrestha, Sampurna. (2017). "PCRAM- Phase Change Memory". Computersciencementor | Hardware, Software, Networking and programming. 4 April 2021. computersciencementor.com/pcram

 	• (2019, February, 19). “STT-MRAM: Introduction and market status.” Retrieved From: https://www.mram-info.com/stt-mram

	• (2017). “Evaluating ReRAM technology choices for cloud and data center applications” Embedded Computing. Retrieved From: https://www.embeddedcomputing.com/application/misc/evaluating-reram-technology-choices-for-cloud-and-data-center-applications 

	• Lapedus, M. (2017). “What Happened To ReRAM?” Semiconductor Engineering. Retrieved From: https://semiengineering.com/what-happened-to-reram/]

	• Kultursay, E., Kandemir, M., Sivasubramaniam, A., Mutlu, O. “Evaluating STT-RAM as an Energy-Efficient Main Memory Alternative.” Retrieved From: https://users.ece.cmu.edu/~omutlu/pub/sttram_ispass13.pdf
	
	• Market Study Report “Next generation non-volatile memory (NVM) technologies Market Trend, COVID-19 Impact, Current Industry Figures With Demand By Countries And Future Growth 2026” Just Positivity (2021) https://justpositivity.com/next-generation-non-volatile-memory-nvm-technologies-market-6962

	• Sun G., Zhao J., Poremba M., Xu C. & Xie Y. “Memory that never forgets: emerging nonvolatile memory and the implication for architecture design” National Science Review (2018) https://academic.oup.com/nsr/article/5/4/577/4093905?login=true 

	• Angelini C. “3 emerging memory technologies that will change how you handle big data”  Venture Beats (2019) https://venturebeat.com/2019/11/13/3-emerging-memory-technologies-that-will-change-how-you-handle-data/ 



