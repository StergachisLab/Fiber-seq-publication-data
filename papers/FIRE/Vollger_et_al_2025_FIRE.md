# Epigenetic data used in <ins>F</ins>iber-seq <ins>I</ins>nferred <ins>R</ins>egulatory <ins>E</ins>lements (FIRE) publication

All epigenetic data used in the FIRE publication is available on AWS as a public dataset at the following URL:

- [https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE](https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE])

Results are organized at the top level by sample, e.g.:

- [https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE/GM12878](https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE/GM12878)

## Structure of the results

The structure of the results within each of these folders is then uniform with the following important files (using GM12878 as the example sample):

| File                                          | Description                                                               |
| --------------------------------------------- | ------------------------------------------------------------------------- |
| GM12878/FDR-peaks/FDR-FIRE-peaks.bed.gz       | FIRE peaks called at FDR 0.05                                             |
| GM12878/FDR-peaks/FDR.track.bed.gz            | FIRE coverage and FDR values for the whole genome                         |
| GM12878/hap1-vs-hap2/FIRE.hap.differences.bed | Differences in FIRE peaks between haplotypes                              |
| GM12878/fiber-calls/FIRE.bed.gz               | Individual FIREs called from single molecule fiber-seq data               |
| GM12878/trackHub/hub.txt                      | Track hub for visualizing all the FIRE results in the UCSC genome browser |

## FDR FIRE peaks file

Description of columns you will find in the FDR FIRE peaks file:

| Column         | Description                                                             |
| -------------- | ----------------------------------------------------------------------- |
| #chrom         | Chromosome of the peak                                                  |
| peak_start     | Start of the peak                                                       |
| peak_end       | End of the peak                                                         |
| start          | Start of the maximum of the peak                                        |
| end            | End of the maximum of the peak                                          |
| coverage       | Coverage of the peak                                                    |
| fire_coverage  | Coverage of the FIREs in the peak                                       |
| score          | FIRE score of the peak                                                  |
| \*{H1,H2}      | Repeats of previous columns but specific for each of the two haplotypes |
| FDR            | False discovery rate of the peak                                        |
| log_FDR        | -10\*log10 of the FDR                                                   |
| FIRE_size_mean | Mean size of the FIREs in the peak                                      |
| FIRE_size_ssd  | Standard deviation of the size of the FIREs in the peak                 |
| FIRE_start_ssd | Standard deviation of the start of the FIREs in the peak                |
| FIRE_end_ssd   | Standard deviation of the end of the FIREs in the peak                  |
| pass_coverage  | Whether the peak passes coverage filters                                |

## UCSC track hubs

We include UCSC trackHubs for each sample at the following URL and we also have a description of the trackHub [here](https://s3-us-west-2.amazonaws.com/stergachis-public1/Mitchell/temp/FIRE/dev/trackHub/fire-description.html):

- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/GM12878/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/30X_GM12878/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/K562-PS00075/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00338_COLO829BL_1/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00356_COLO829BL_2/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/COLO_T_2_PS00_418_451_488/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00272/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00321/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00327/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00381/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00382/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00383/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00384/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00389/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00392/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00404/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00422/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00456/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00459/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00465/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00468/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00471/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00476/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00479/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00482/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/PS00485/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/ST001-liver/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/ST001-lung/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/UDN318336_PS00189/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/UDN633333_PS00115/trackHub/hub.txt
- https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/HG002/trackHub/hub.txt
