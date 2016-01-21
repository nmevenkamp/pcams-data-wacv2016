------------------ Instructions for executing the quantitative evaluation on the Outex results ------------------

The quantitative evaluation of the Outex segmentations (seg000.png - seg099.png) is done
by the "quocGCC/finishedProjects/highDimFeatureSegmentation/Run_Evaluation_Outex" executable
with the following usage: Run_Evaluation_Outex <segmentationDirectory> <pathToGroundTruthSegments>

The quantitative measures are stored in a .txt file inside the <segmentationDirectory>.


IMPORTANT NOTE: Run_Evaluation_Outex requires the Hungarian external library in order to match segments
				in the ground truth to those detected by the segmentation algorithm.
				
				To connect the source code with the Hungarian external library,
				add "-DBUILD_AND_USE_HUNGARIAN=1" to "quocGCC/go.sh" and execute the bash script again.
				This should automatically download and link the library.
				
				In case this does not work, try downloading the Hungarian library manually from
				http://robotics.usc.edu/~lantao/codes/hungarian-v2.0.zip
				and place all of its .h and .cpp files inside
				"quocmesh/external/hungarian-source".
				Then, re-run the "quocGCC/go.sh" bash script.


