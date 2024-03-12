## The Iterative Threshold-Seeking Algorithm (ITSA)
#### By: DrAKLab team led by Wong, AKO 
#### Project funded by @CIHR and @ArthritisSociety

For application to MR Images of muscle. The code provided here is adapted for analysis of 
T1-weighted Fast Spin Echo (FSE) images of the thigh from the Osteoarthritis Initiative (OAI)

Run execution notebook to go through workflow 
Definitions notebook contains all work flow procedures 

Algorithm goes through: 
1) Inhomogeneity correction (CLAHE)
2) Thigh separation (assuming both legs are scanned) into left and right thighs
3) Background removal
4) Subcutaneous fat removal using snake algorithm and correcting fat excluded from muscle mask
5) Muscle mask isolation by removing femoral bone and marrow
6) Initial thresholding and ITSA optimization of threshold
7) Round 1 and 2 of ITSA application
8) With Round 2 3D connectivity check and partial volume correction
9) Quality control check and exporting Sliceomatic tags for manual correction
10) Reimporting corrected tags
11) Computation of IMF metrics

    
