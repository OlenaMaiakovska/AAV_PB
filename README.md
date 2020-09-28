# AAV_PB
Here I publish the description and the basic workflow for PacBio Sequencing data analysis


The SMRT sequencing platform utilizes a sequencing-by-synthesis approach, when DNA polymerase incorporate the fluorescently labelled nucleotides into native DNA strands in a real-time fashion. The DNA polymerase is anchored to the bottom of the sequencing unit called zero-mode waveguide (ZMW). ZMW provides the smallest volume for the light detection during the synthesis reaction. On 3000 of ZMWs were allocated on prototype chip called SMRT cell, where the replication process was parallelized in ZMWs. 

The recorded  “movie” of light pulses from each ZMW can be interpreted into sequence of bases, which represents a continuous long read (CLR) (Eid et al. 2009). The process of sequencing lasts in dependance of the polymerase lifetime and usually reaches the read length of ~ 40 Kb. However, the sequencing error rates is high and reach 15%, which is the frequent phenomena in TGS reads (Lee et al. 2016). These highly erroneous long reads can be improved by the generation of multiple subreads from CLR via specific modification of DNA fragments. The hairpin adapters are ligated at both ends of the double stranded DNA (dsDNA) fragment and allow the formation of the circular template, which has to be sequenced by attached DNA polymerase in the multiple passes. The subreads with about 15% of error rate used for generation of consensus highly accurate reads referred as “Circular Consensus Sequences” (CCS). The long and accurate reads enabled the identification of small and large sequence variations in the genome, as well as their successful application in the de novo genome assembly. The recent optimisation of CCS generation resulted in 99.8% accuracy for long high-fidelity reads (HiFi), but with the reduces average read length (13.5 kb) (Wenger et al. 2019). 

PacBio company successfully develop the single-molecule real-time sequencing and increase the throughput and the cost-effectivity. Thus, Sequel I platform has the SMRT cell with 1 M of ZMWs and was recently replaced by Sequel II platform, which delivers about 8X more reads with 8 million ZMWs per SMRT Cell. 


![Generation of circular consensus sequence](https://www.nature.com/articles/s41587-019-0217-9/figures/1) 



