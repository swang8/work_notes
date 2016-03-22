## MinION portable sequencer from nanopore tech
### How dose it work [ref: [Ref](https://nanoporetech.com/science-technology/how-it-works)]
A nanopore is a nano-scale hole. In its devices, Oxford Nanopore passes an ionic current through nanopores and measure the changes in current as biological molecules pass throug the nanopre or near it. The information about the change in current can be used to identify that molecule.
#### Nanopore
A protein nanopore is set in an electrically resistant polymer membrane. An ionic current is passed through the nanopore by setting a voltage across this membrane. If an analyte passes through the pore or near its aperture, this event creates a characteristic disruption in current. Measurement of that current makes it possible ot identify the molecule in question. For example, this system can be used to distinguish between the four standard DNA bases G, A, T and C, and also **modified bases** (methylated?).
#### Array of Microscaffolds
An array of microscaffolds holds the membrane in which the nanopore embedded. This keeps the membrane stable during shipping and usage. (what temperature can it tolerate? Shake resistant?)
#### Array Chip
Each microscaffold on the sensor array chip contains an individual electrode, allowing for multiple nanopore experiments to be performed in parallel. Sensor arrays may be manufactured with any number of channels.
#### ASIC
Each nanopore channel is controlled and measured by an individual channel on a corresponding, bespoke Application Specific Integrated Circuit (ASIC). More than one ASIC may be included in a device and Oxford Nanopore is building ASICs of different sizes for different purposes.

#### Workflow versatility: no fixed run time [Ref](https://nanoporetech.com/science-technology/workflow-versatility-no-fixed-run-time/workflow-versatility-no-fixed-run-time)
A key feature of the MinION device, the PromethION and the GridION system is that there is no fixed run time. A user can run any of the systems for a short or long period of times as data is streamed in real time. This can enable real-time analyses so that the user can predetermine an experimental endpoint and run the system for as long as it takes to collect sufficient data to address that question.

### Performance, [Assessing the performance of  the Xoford Nanopore Technologies MinION, March 2015](http://www.sciencedirect.com/science/article/pii/S2214753515000224)
Great technology, but how is its performance in terms of accuracy?
#### Abstract of the paper
MinION was used to re-sequence three bacterial genomes. By comparing to MiSeq reads for the same genome, the estimated error rate is **38.2%**, Mean and median read lenghts were 2Kb and 1Kb. 
These are not exciting numbers at all. I guess error correction would be necessary for these high error rate reads to be useful. Something similar to what people have been doing for PacBio long reads.
#### Tools used in the paper
1. Poretools, to convert sequencing data into fastq/a;
2. LAST alignment tool, to align MinION reads to referece;
3. BWA mem for long-reads alignment

### More tools for nanopore sequencing data anlaysis
[See this link](http://nextgenseek.com/2015/10/software-tools-for-oxford-nanopore-sequence-data/)


[Shichen, 03/22/2016]
