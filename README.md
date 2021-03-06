### Data and results: Variational Multi-Phase Segmentation using High-Dimensional Local Features
Data and results used in our paper presented at the **IEEE Winter Conference on Applications of Computer Vision (WACV 2016)** - see reference below.
___
**CONTENTS**:
- Outex_US_00000 texture segmentation test suite (converted to .png format)
- Crystal images (grains with 1,2 and 3 segments, CMS-GaAs two-phase crystal)
- Link to ICPR 2014 contest dataset
- All corresponding segmentations produced by our method PCA-MS
 
___
    |- data/
    |+ - Crystals               ground truth crystal images (Figure 2)
    |+ - ICPR2014               README.txt with link to the ICPR 2014 contest dataset
    |+ - Outex:                 ground truth segments and texture mosaics
    |                           from the Outex_US_00000 test suite converted from .ras to .png
    |- results/
    |+ - Crystals               segmentations (.png) and boundary curves (.pdf) 
    |+ - ICPR2014               segmentation results used in Table 2
    |+ + - Raw                  before TxtMerge post-processing
    |+ + - TxtMerge             after TxtMerge post-processing
    |+ + - README.txt           link to Prague website with benchmark results
    |+ - Outex                  segmentation results used in Table 1
    |+ + - README.txt           instructions on how to run quantitative evaluation
    |+ + - Clustering           k-means clustering
    |+ + - FSEG_ICPR2014        ICPR2014 version of FSEG (see link below)
    |+ + - FSEGstar             FSEG with adjusted spectral histograms (see paper)
    |+ + - FSEGstar-TxtMerge    FSEGstar without TxtMerge post-processing   
    
The comparison with FSEG is based on the [ICPR 2014 version](http://web.ornl.gov/~jiy/FSEG_contest.zip).
___
**QUANTITATIVE EVALUATION**:
 - ICPR 2014 benchmark: [The Prague Texture Segmentation Datagenerator and Benchmark](http://mosaic.utia.cas.cz/index.php?act=view_res&f3=0&id=&dyn=0&vis=7&hr=1&sort=2&dir=0&f1=0&f2=-1&f4=-1&ndl=-1&nt=-2&alg=-1&ver=&bid=3)
 - Outex_US_00000 test suite: [results/Outex/README.txt](results/Outex/README.txt)

___
**REFERENCE**:
Mevenkamp, N., and Berkels, B. _Variational Multi-Phase Segmentation using High-Dimensional Local Features_. Applications of Computer Vision (WACV), 2016 IEEE Winter Conference on, 2016, (accepted)
___
**CONTACT**:<br>
Niklas Mevenkamp<br>
Aachen Institute for Advanced Study in Computational Engineering Science<br>
RWTH Aachen University<br>
mevenkamp@aices.rwth-aachen.de<br>
http://www.aices.rwth-aachen.de/people/mevenkamp
