Getting Started
^^^^^^^^^^^^^^^

**Installation**


  1. Install a full version of MATLAB_

  .. _MATLAB: https://www.mathworks.com/products/matlab.html

  2. Using Git BASH or direct download, clone/download the SpikeClusterAnalyzer repository_ to the Documents>>MATLAB folder (link not available right now)

  .. _repository:

  - To use Git BASH to clone the respository (recommended in order to have a more streamlined method of updating the program), download `Git for Windows`_

  .. _Git for Windows: https://gitforwindows.org/

  - Open *Git for Windows* and navigate to the MATLAB folder:

    ``$ cd Documents/MATLAB/``

  - Clone the *Spike Cluster Analyzer* by typing in 

    ``$ git clone https://github.com/tigsch/SpikeClusterAnalyzer.git``

  - If you have already cloned the repository but wish to update to the newest version of the *Spike Cluster Analyzer*, navigate to SpikeClusterAnalyzer folder: 

    ``$ cd Documents/MATLAB/SpikeClusterAnalyzer/``

    then pull the new version:

    ``$ git pull origin master``

  .. Download and unzip the Spike Cluster Analyzer package here (not available right now)

  .. 3. Drag and drop the entire unzipped folder directly into ~/Documents/MATLAB/ which should have been created after installing Matlab.

  3. Within MATLAB, add all folders within ~/MATLAB/SpikeClusterAnalyzer/ except command_line to the path. Then open MATLAB>>SpikeClusterAnalyzer>>GUI

  .. line 46

  4. Launch *analyzer* from MATLAB command line

  ..

**Preparing files for analysis**


This is for anyone who has analysis files from using the `2013 Analyzer`_ and wishes to do further analysis or adjustments of the clusters found previously.

.. _2013 Analyzer: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3988315/

  1. Ensure that all EEG recording (.mat) files are organized at the desired location. The original output folders are fine for this, but all the resulting files from the analysis will be located in the same folder, so be aware of this.

  ..

  2. Any .txt files files output from the original 2013 Analyzer should be pasted into Excel or similar program, and apply Text-to-columns delimited by space. Ensure that the first column contains only Date and the second column Time. Some versions of the old Analyzer include other data in the first few columns which can be deleted (save an extra copy first, if desired).
  
  ..
  
  3. In case any sorting was done to this data, such as to check the effects of laser on/off, ensure that the data is sorted back into chronological order before using it within the *Spike Cluster Analyzer*.


