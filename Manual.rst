Instruction Manual
------------------

..

**Table of Contents**

1. `Getting Started`_

2. `Initial analysis of EEG data`_

  `Using analysis output from the 2013 Analyzer`_

  `Using new EEG recordings`_

3. `Secondary analysis of clusters`_

4. `Cross analysis of subjects`_

5. `Spike analysis`_

6. `Troubleshooting`_ 



.. _Getting Started: 

1. Getting Started
^^^^^^^^^^^^^^^^^^

**Installation**


  1. Install a full version of MATLAB_

  .. _MATLAB: https://www.mathworks.com/products/matlab.html

  2. Using GitBash or direct download, clone/download the SpikeClusterAnalyzer repository_ to the Documents>>MATLAB folder (link not available right now)

  .. Download and unzip the Spike Cluster Analyzer package here (not available right now)

  .. _repository:

  .. 3. Drag and drop the entire unzipped folder directly into Documents>>MATLAB which should have been created after installing Matlab.

  3. Within MATLAB, add all folders except command_line to the path. Then open MATLAB>>SpikeClusterAnalyzer>>GUI.

  .. line 46

  4. Launch "analyzer" from MATLAB command line.

  ..

**Preparing files for analysis**


This is for anyone who has analysis files from using the `2013 Analyzer`_ and wishes to do further analysis of the clusters found previously.

.. _2013 Analyzer: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3988315/

  1. Ensure that all EEG recording (.mat) files are organized at the desired location. The original output folders are fine for this, but all the resulting files from the analysis will be located in the same folder, so be aware of this.

  ..

  2. Any .txt files files output from the original 2013 Analyzer should be pasted into Excel or similar program, and apply Text-to-columns delimited by space. Ensure that the first column contains only Date and the second column Time. Some versions of the old Analyzer include other data in the first few columns which can be deleted (save an extra copy first, if desired).


.. _Initial analysis of EEG data:

2. Initial analysis of EEG data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. _Using analysis output from the 2013 Analyzer:

**Using analysis output from the 2013 Analyzer**

  .. line 79
     
  1. Ensure that *load cluster data* is unchecked, and then open a Recording (.mat) file.

  ..

  2. Click on **Semi-Auto** >> **Settings**

  ..

  3. Under settings, set the channel to the correct one, and then also click on "Ch1" and scroll until you reach the corresponding channel

  ..

  4. Click on **Refine** >> Pick the Excel file that contains the analysis data >> Specify which sheet contains the correct data

  ..

  5. Select a template, currently found in GUI>Others>test_data>template cluster file

  .. line 101

  6. If this is done correctly, the program will begin processing

  ..

  7. The new cluster file, which has the same name as the recording file plus _\cluster, should be saved in the same location as the recording file *Request - have this default to the same folder the recording is pulled from*

  ..

  8. Make a copy of the cluster file, if desired, if you plan to mark additional clusters or delete previously marked ones

  ..

  9. Analysis will be loaded. Check the box for **ps** to see the overlay if this does not automatically occur. If no further cluster identification is needed, skip to step 11. If you need to zoom out, change the **Display Window** to a larger number, such as 200. Do not click on Update Display Window when doing this.

  ..

  10. To add extra clusters, *right* click **Refine**, this should turn the button red

      * *shift-click* to add new start and stops to new clusters
      * *shift-doubleclick* in between markers to delete clusters
      * when finished, click **SaveCF** (save cluster file), and right click on **Refine** to turn the function off

  11. Continue to `secondary analysis`_ of clusters

  .. line 130

  ..

.. _Using new EEG recordings:

**Using new EEG recordings**

  ..  

  *This feature currently not working!! Errors out at Step 9*

  1. Load recording (.mat) file, making sure **load cluster data** is unchecked

  ..

  2. Create a credential file: Click on **1) Credential** and fill in the subject information, at least the ID. Save this file to the same location as the recording 

  ..

  3. Create a settings file: Click on **Semi-Auto** then **Settings**. Load a settings file (.one). Use an old one from a previous subject or recording, if desired.

  .. line 153

  4. To adjust settings, scroll through the recording until you find a cluster (and some artifact, ideally) and click on **1) Window**

  ..

  5. Click on **Apply Settings**

     - To produce plots while these settings are applied, before clicking on **Apply Settings**, select **Plot** (on the far right)
     - In the new window, click on **Cluster Detection** and **Compare Clusters**, close window
     - Click on **Apply Settings**
     - This should cause different plots showing clusters detected using different criteria. When finished, click **DelW** to close all plots

  ..

  6. If the results observed in the plots are satisfactory, click **Save Settings** and name the file with the subject ID (or any other name) and save to the same location as the recordings and credential file.

  ..  

  7. If the results need to be adjusted, change the criteria within the section *Spike detection* and click **Apply Settings** again *what about the pattern section?*

  .. 

  8. Make sure the credentials (.cre), settings (.one), and all recording files for the same subject that you wish to analyze are in the same folder. (MAKE SURE THERE IS NO _\cluster FILE)

  ..

  9. Click **Step1**. Set number of points as the number of data points that should have been sampled during the recording (at a sampling rate of 1000 Hz, this should be 3600 sec times 1000 = 3.6e6). When the processing is done, there should now be a _\cluster file for each recording file in the folder.

  ..

  10. At this point, each recording's set of detected clusters can be checked and adjusted manually using the **Refine** feature (described in step 7 and onwards in the previous section) 

.. _secondary analysis:
.. _Secondary analysis of clusters:

3. Secondary Analysis
^^^^^^^^^^^^^^^^^^^^^

Once a cluster file (_cluster.mat) has been made for a specific recording, this next analysis is run in order to set the spike detection thresholds for individual seizures and output information regarding all spikes within each cluster. This can be done using **AnalysisB**.

  1. Click **AnalysisB** >> Name the folder with any name to indicate this is the analysis output for this file

  ..

  2. The program will enter a new mode which brings up the first marked cluster. 

    * If the individual spike identification is satisfactory, click *Yes* to move to the next seizure
    * *No* will accept your current thresholds and apply them to the rest of the clusters
    * Click *modify* to readjust the detection threshold by dragging the black and red lines to the desired locations (black is negative threshold, red is positive)

  3. After the final cluster is adjusted, a plot will pop up showing all clusters overlaid onto the recording. This window can now be closed and the next recording can be opened for analysis.



.. _Cross analysis of subjects:

4. Cross analysis of subjects
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Once all the desired recording files have been analyzed, the next step is to compare between groups. I haven't done this yet so this will be written once I try it out.


.. _Spike Analysis:

5. Spike Analysis
^^^^^^^^^^^^^^^^^

Will be written once I've tried this feature out.


.. _Troubleshooting:

6. Troubleshooting
^^^^^^^^^^^^^^^^^^

At the moment the best way to solve incidental errors is to reboot the analyzer. If you have to reboot anytime after you have already created your cluster file, follow these steps:

  1. Close MATLAB Analyzer window

  .. 

  2. Run *analyzer*

  ..

  3. Once the Analyzer has launched, click on **load cluster data**

  ..

  4. Click **Open File** and open the desired MATLAB recording file

  ..

  5. Click on **ps** to view the previously saved clusters

  ..

  6. Depending on which step you were on when the error happened, you may have to run **Refine** or **AnalysisB** once again

