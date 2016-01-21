------------------ Instructions for executing the quantitative evaluation on the Outex results ------------------

The quantitative evaluation of the Outex segmentations (seg000.png - seg099.png) is done
by the "quocGCC/finishedProjects/highDimFeatureSegmentation/Run_Evaluation_Outex" executable
with the following usage: Run_Evaluation_Outex <segmentationDirectory> <pathToGroundTruthSegments>

The quantitative measures are stored in a .txt file inside the <segmentationDirectory>.


PLEASE NOTE:

Run_Evaluation_Outex requires the Hungarian external library in order to match segments
in the ground truth to those detected by the segmentation algorithm.
Normally, the library should be downloaded and built automatically when you execute "quocGCC/go.sh".

If this is not the case, i.e. you get an exception like the following:
"This executable requires the Hungarian external library. Please refer to the README.txt located inside the same source code folder as this executable for further instructions."
then try the following:

1) inside the "quocGCC/go.sh", check whether the flag  "-DBUILD_AND_USE_HUNGARIAN=1" is set; otherwise, add it and re-run go.sh

2) try downloading the Hungarian library manually from
http://robotics.usc.edu/~lantao/codes/hungarian-v2.0.zip
and place all of its .h and .cpp files inside "quocmesh/external/hungarian-source".
Then, re-run the "quocGCC/go.sh" bash script.


