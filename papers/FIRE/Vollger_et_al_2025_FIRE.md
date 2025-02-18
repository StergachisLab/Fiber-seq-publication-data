# Epigenetic data used in the FIRE publication

All epigenetic data used in the FIRE publication is available on AWS as a public dataset at the following URL:

- [https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE/]()

Results are organized at the top level by sample, e.g.:

- [https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/index.html?prefix=2024/Vollger_et_al/FIRE/GM12878/]()

## Structure of the results

The structure of the results within each of these folders is then uniform with the following important files (using GM12878 as the example sample):

| File                                          | Description                                                               |
| --------------------------------------------- | ------------------------------------------------------------------------- |
| GM12878/FDR-peaks/FDR-FIRE-peaks.bed.gz       | FIRE peaks called at FDR 0.05                                             |
| GM12878/FDR-peaks/FDR.track.bed.gz            | FIRE coverage and FDR values for the whole genome                         |
| GM12878/hap1-vs-hap2/FIRE.hap.differences.bed | Differences in FIRE peaks between haplotypes                              |
| GM12878/fiber-calls/FIRE.bed.gz               | Individual FIREs called from single molecule fiber-seq data               |
| GM12878/trackHub/hub.txt                      | Track hub for visualizing all the FIRE results in the UCSC genome browser |

# UCSC track hubs

- [https://s3-us-west-1.amazonaws.com/stergachis-manuscript-data/2024/Vollger_et_al/FIRE/GM12878/trackHub/hub.txt]()
