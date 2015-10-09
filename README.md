The work is described in the following publication: 

Balazs Szigeti, Ajinkya Deogade, Barbara Webb: Searching for motifs in the behaviour of larval Drosophila and C. elegans reveals continuity between behavioural states.

Accepted at:
Preprint:

Please cite it if you use any of this code for a publication/presentation!

As this code is presented for the sake of methodological repeatability, the use of this software is at your own risk. The authors are not responsible for any damage that may result from errors in the software. Downloaders of this software are free to use, modify, or redistribute this software how they see fit, but only for non-commercial purposes and all modified versions may only be shared under the same conditions as this. This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/.

Notes

The input to this code is the eigenshapes coefficient time series. Machine vision code to extract the midlines from videos have not been included as each camera/illumination combination produces different images
The CCtoolbox folder includes code that was not produced by me, this is the spline regression clustering algorithm, here is the original publication: Joint Probabilistic Curve Clustering and Alignment. The curve_clust.m function have been modified from the original code. The change was made to make the motif detection symmetric with respect to positive and negative peaks in the eigenshape time series. This symmetry corresponds to the dorsal/ventral symmetry in worm behaviour and the lateral symmetry in maggot behaviour 
peakfinder.m is not my work, see code for credits
The data used for this publication is available at: http://tinyurl.com/p7eculs

Workflow:
Once the eigenshape time series is ready the data should be structured as in the example data files (e.g. CSAgar01.mat). The fields are explained in the input/output of various functions. Once you have your data ready apply the appropriate action segmentation algorithm (worm/maggot). Next run the  runCC.m (CCtoolbox folder) to build the statistical model of the data. The final models that I have created (and the data at the intermediate steps) is available along with the original data  at http://tinyurl.com/p7eculs

For any further questions or bug report about this code, please email Balazs Szigeti: 
b{dot}szigeti{at}sms{dot}ed{dot}ac{dot}uk
