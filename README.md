# GWSBE
Regenerated Rice Re-sequencing to evaluating genome-wide specificity of base editors

This is the pipiline for this paper.



1.first Clean fastq file using 1.Clean.sh ;
  please set the the R1,R1,Sample,core at the top of shell,Then use this command:

   sh 1.clean.sh

2.using bwa to mapping the reads to the Refgenome;
  The RefGenome ZH11 can be download at http://mbkbase.org/ZH11/;
 
   sh 2.bwa.sh
 
  The mapping result will in the tmp_pipe_data file;
  The *.realigned.bam is the bam file use for GATK,Lofreq and strelka2;
3.Call SNV/Indel use GATK,Lofreq and Strelka2;
  