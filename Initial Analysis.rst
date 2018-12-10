Initial analysis
^^^^^^^^^^^^^^^^

`If you have analysis pre-existing from the 2013 Analyzer`_

`If you have not yet analyzed your EEG recording file`_


.. _If you have analysis pre-existing from the 2013 Analyzer:

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

  11. Continue to secondary analysis of clusters

  .. line 130

  ..

.. _If you have not yet analyzed your EEG recording file:

**Using new EEG recordings**

  ..  

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

  7. If the resulting cluster results are not satisfactory and need to be adjusted, change the criteria within the section *settings* within the Analyzer and click **Apply Settings** again to re-plot the cluster detection using the new settings. The plots made can be adjusted based on which settings were changed. For example, if the thresholds are being adjusted in *settings*, then it maybe appropriate to just plot *Spike Detection - 1st Threshold*. 

  .. 

  8. Make sure the credentials (.cre), settings (.one), and all recording files for the same subject that you wish to analyze are in the same folder. (MAKE SURE THERE IS NO _\cluster FILE)

  ..

  9. Click **Step1**. Set number of points as the number of data points that should have been sampled during the recording (at a sampling rate of 1000 Hz, this should be 3600 sec times 1000 = 3.6e6). When the processing is done, there should now be a _\cluster file for each recording file located inside a folder called *Step1_Channel_##_yourname*

  ..

  10. At this point, each recording's set of detected clusters can be checked and adjusted manually using the **Refine** feature (described in step 7 and onwards in the previous section) 


