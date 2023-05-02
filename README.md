# mutationathon
Supplemental code for L.A. Bergeron, S. Besenbacher, T.N. Turner, C.J. Versoza, R.J. Wang, A.L. Price, E. Armstrong, M. Riera, J. Carlson, H. Chen, M.W. Hahn, K. Harris,  A.S.L.N.M. Kleppe, E.H. López-Nandam, P. Moorjani, S.P. Pfeifer, G.P. Tiley, A.D. Yoder, G. Zhang, M.H. Schierup. 2022. **The mutationathon highlights the importance of reaching standardization in estimates of pedigree-based germline mutation rates.** *eLife*, 11: e73577.

CV's DNM detection pipeline:
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


Datasets are available from BioProject PRJNA588178 (Bergeron *et al.* 2021).
