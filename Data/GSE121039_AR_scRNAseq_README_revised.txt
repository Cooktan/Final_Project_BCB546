Data are from isolated single pre-meiotic and maize meiotic cells. Sequencing libraries were constructed with the CEL-Seq2 protocol, modified by splitting cell lysates into two tubes before processing to construct split-cell technical replicates. In total, there are 216 cells with 2 split-cell technical replicates each in this dataset. Library prep was randomized at several stages and so every split-cell sample is spread across multiple Illumina libraries.

To de-multiplex this dataset, refer to the barcoding scheme in the associated 'cell metadata.csv' file. The file 'cell metadata.csv' contains a table listing all split-cell samples and the two barcodes that uniquely identify that sample: a 6-7 nt CelSeq2 barcode and an Illumina barcode (RPI1-29). Raw fastq files and GEO samples are named by the Illumina barcode (RPI1-29) and the lane used for sequencing (Lane 1 and Lane 2). CelSeq2 barcodes are internal to Read 1 of each paired end library:

*Read 1* contains a 10 nucleotide (nt) unique molecular identifier (UMIs), a 6-7 nt CelSeq2 sample barcode, and a 24 nt poly T stretch from the reverse transcription primer:

5': NNNNNNNNNNCCCCCC(C)TTTTTTTTTTTTTTTTTTTTTTTTxxxxxxxxxx......

where Ns designate the UMI, Cs designate the 6-7 nt CelSeq2 sample barcode, and xs are transcript sequence starting from the end of the 3' untranslated region (in reverse orientation).

*Read 2* of each paired end read contains transcript sequence. This library is directional and read 2 is in the same direction as the original mRNA transcript.

The CelSeq2 barcodes used were:

name:	sequence:
dT_1s	AGACCTC
dT_2s	AGCTAG
dT_4s	AGCTTC
dT_5s	CATGAG
dT_6s	CATGCA
dT_9s	CAGATC
dT_10s	TCACAG
dT_19s	TCGATC
dT_23s	GTCTAG
dT_25s	GTTGCA
dT_26s	GTGACA
dT_31s	ACTCGA
dT_37s	CTAGGA
dT_46s	TGCAGA
dT_101X	TCACGC
dT_102X	GAGTCG

Primer dT_4s did not produce usable sequence and it is recommended to exclude samples with this primer.
