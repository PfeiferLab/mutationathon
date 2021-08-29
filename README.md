# mutationathon
CV's DNM detection pipeline published as part of "Mutationathon: towards standardization in estimates of pedigree-based germline mutation rates" (Bergeron *et al.*, BioRxiv).
* **step 2: Alignment and post-alignment processing**
* **step 3: Variant calling**
* **step 4: Detecting DNMs**
  
  *Filter criteria and their thresholds:*
  * *autosomal biallelic SNPs fully genotyped in the extended trio*
  * *GATK Best Practices hard filter criteria*
  * *Mendelian violation where parents were HomRef and offspring was Het*
  * *0.5 × DP<sub>ind</sub> & 2 × DP<sub>ind</sub>*
  * *0.25 <= AB <= 0.75*
  * *GQ >= 40*
  * *AD<sub>alt</sub> = 0 in parents*

  *CG: filter criteria and thresholds used to identify DNM candidates were applied to the BP resolution .vcf (if applicable)* 


Datasets are available from BioProject PRJNA588178 (Bergeron *et al.* 2021); for additional details, see Bergeron *et al.* BioRxiv.
