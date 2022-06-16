# Amazing-Varient-Annotation
## 1. 1000 Genomes [https://doi.org/10.1038/nature15394]
## Find most genetic variants with frequencies of at least 1% in the populations studied and to capture the allele frequencies for all 26 populations as well as the 5 super populations and the total population.
### Parse the VCF file and extract the following fields from INFO:
```
AA
AC
AN
EAS_AN
AMR_AN
AFR_AN
EUR_AN
SAS_AN
EAS_AC
AMR_AC
AFR_AC
EUR_AC
SAS_AC
```
### JSON Output:
```
"oneKg":{
   "allAf":0.200879, (allele frequency for all populations. Range: 0 - 1.0)
   "afrAf":0.210287, (allele count for all populations. Integer.)
   "amrAf":0.139769, (allele number for all populations. Non-zero integer)
   "easAf":0.275794,
   "eurAf":0.181909,
   "sasAf":0.173824,
   "allAn":5008,
   "afrAn":1322,
   "amrAn":694,
   "easAn":1008,
   "eurAn":1006,
   "sasAn":978,
   "allAc":1006,
   "afrAc":278,
   "amrAc":97,
   "easAc":278,
   "eurAc":183,
   "sasAc":170
}
```
allAn	int	allele number for all populations. Non-zero integer.
afrAf	float	allele frequency for the African super population. Range: 0 - 1.0
afrAc	int	allele count for the African super population. Integer.
afrAn	int	allele number for the African super population. Non-zero integer.
amrAf	float	allele frequency for the Ad Mixed American super population. Range: 0 - 1.0
amrAc	int	allele count for the Ad Mixed American super population. Integer.
amrAn	int	allele number for the Ad Mixed American super population. Non-zero integer.
easAf	float	allele frequency for the East Asian super population. Range: 0 - 1.0
easAc	int	allele count for the East Asian super population. Integer.
easAn	int	allele number for the East Asian super population. Non-zero integer.
eurAf	float	allele frequency for the European super population. Range: 0 - 1.0
eurAc	int	allele count for the European super population. Integer.
eurAn	int	allele number for the European super population. Non-zero integer.
sasAf	float	allele frequency for the South Asian super population. Range: 0 - 1.0
sasAc	int	allele count for the South Asian super population. Integer.
sasAn	int	allele number for the South Asian super population. Non-zero integer.
