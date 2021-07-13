# This program needs to be run twice: one time with RGB inputs, and second time with optical flow inputs.
# To create mean and standard deviation statistics, the learn_trainingsubset_statistics.py needs to be called for RGB and optical flow separately. The resulting .npy file will have to be named correspondingly. The file name string is used as a parameter in vvad_train.py, vvad_test.py and vvad_fusion_test.py, where 2 separate .npy files are necessary.
# data_dda is a folder with a very small example subset from the TCD-TIMIT preprocessed data. Full preprocessing code is available in a separate repository at: <...> After the preprocessing, the full dataset has to follow the structure of the data_dda folder in this repository.
# The train is started by running vvad_train.py 
# You can then test without any fusion by running vvad_test.py
# The RGB and optical flow models need to be saved and fused with the help of vvad_fusion\_test.py
# Code related to audio label inference is available in the "processing" folder/module
# All other helper utility functions are available in utils.py