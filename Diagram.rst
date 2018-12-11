Glossary
--------

1. Recording File
^^^^^^^^^^^^^^^^^

1. Open File - Opens .mat file containing EEG data from previous recorders

2. Next/Prev File - Left-click opens the previous recording file in the same folder, if available. Right-click opens the next file

3. Load cluster data - Applies the cluster data available as a _\cluster.mat file to the corresponding recording file

4. Load state data - ??

5. Display Window (s) - Changes the view of the recording within the analyzer. The number specifies the length of time shown in the window.

6. Update Display Window - ??


2. Tasks
^^^^^^^^

1. CREDENTIALS - Input and save information about the subject of the recording (.cre file)

2. ANALYSIS A - Initial analysis for detection and adjustment of clusters

   - MANUAL - Mode to input the start and stop of clusters manually

   - SEMI-AUTO - Mode to automatically detect clusters after setting parameters

     * SETTINGS

       #. OPEN SET - Open previous settings (from another timepoint or another subject)

       #. WINDOW - Sets the boundaries of the data to the current viewing window

       #. APPLY SET - Applies all settings (specified in **4a**) to the current viewing window to detect clusters

       #. SAVE SET - Saves settings (.one file) 

     * Step1 - Applies settings saved in **3) SAVE SET** to entire current file and all other recording files within the same folder

     * REFINE - Allows adjustment and deletion/creation of cluster markers made during the MANUAL, SEMI0AUTO, and AUTO modes

   - AUTO - Still in progress

3. ANALYSIS B - Utilizes recording and cluster file to allow a secondary adjustment to threshold settings for previously detected clusters

4. COLLECTION - ??


3. Video
^^^^^^^^

1. Play Video - Plays the recording's corresponding video according to the length of the viewing window

2. Video1 - Click to rotate through different videos

3. 1x - Speed of video?

4. CamCtrl - ??


4a. Settings
^^^^^^^^^^^^

1. Settings for channel - Self explanatory, specify the channel of the recording you will be analyzing

2. Signal

  - filter order - ??

  - cutoff low - ??

  - cutoff high - ??

3. Spike detection

  - thr pos - positive threshold

  - thr neg - negative threshold

  - thr rej - lower threshold for rejecting spikes

  - 2nd (button) - re-analyzes spikes using the 2nd threshold after passing the original thr pos and neg

  - minwidth - minimum width of spike for inclusion

  - maxwidth - maxiumum width of spike for inclusion

  - mindist - minimum distance between spikes (?) for inclusion into cluster

  - thr down ??

  - Peakseek mode ??

4b. Spike Cond
^^^^^^^^^^^^^^

1. Spike Cond

  - run template - ??

2. Artefact rejection - many criteria....??

4c. Cluster detection
^^^^^^^^^^^^^^^^^^^^^

1. neighbor dist (ms) - distance between two clusters in order to be considered separate ??

2. cluster gap (ms) - ??

3. min cluster dur (ms) - minimum cluster duration that defines "short clusters" that are removed by filtering in CLUSTER FILE

4. spike max dist (ms) - maximum distance by which a negative and positive spike can be paired

5. +pre 2nd - ??

6. +post 2nd - ??

4d. Compare clusters
^^^^^^^^^^^^^^^^^^^^

1. overlap thr - the percentage overlap needed to be considered a single cluster (for example, a cluster detected using positive spike thresholds that overlaps 80% with a cluster detected using negative spike thresholds, will be considered one cluster)

2. overlap cond - combination of settings to check for overlap (ps-positive spikes, ng-negative spikes, pr-paired spikes)

3. Mode

  - overlap/dom - only the overlap between clusters will be counted as the new cluster

  - total - the full length of the overlapping clusters will be counted as the new cluster

4e. ?? need a title for this
^^^^^^

1. welch - ??

2. sgram - ??

3. Filter - ??

4. plot - sets which plots will be made during **2) APPLY SET** and **Step 1**

5. cmb - ??

6. run filter - ??


5. Cluster File
^^^^^^^^^^^^^^^

1. CL

  - ps - clusters detected using positive spikes

  - fps - clusters detected using positive spikes filtered to remove short clusters (defined by **min cluster dur**)

  - ng - clusters detected using negative spikes

  - fng - clusters detected using negative spikes filtered to remove short clusters

  - pr - clusters defined using pairs of negative and positive spikes (defined using **spike max dist** in 4c and thresholds in 4a)

  - fpr - clusters defined using pairs of negative and positive spikes, filtered to remove short clusters 

  - vdom - clusters formed from merges of different criteria (ps/ng/pr) defined using **4d) Compare clusters**

  - vfdom - clusters found using vdom, filtered to remove short clusters

2. CRSR - ??

3. SaveCF - Saves CF after going through **Refine** to adjust clusters

4. LoadCF - ?? loads cluster file?

5. SaveCF_NC - ??

6. Clear All CL - clears all clusters from the screen??

7. Clear all - ??

8. Clear noshorts - ??

9. Clear shorts - ??


6. Template Matching
^^^^^^^^^^^^^^^^^^^^

1. Pattern - ?? 

2. Save Temp - ??

3. Save Mtemp - ??

4. Clear Temps - ??


7. Spike Analysis
^^^^^^^^^^^^^^^^^

1. SpikeDet - ??

2. Spike GUI - ??

3. OSC - original sampling rate ??


8. Recording Viewer Settings
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. DelW - Closes all plot windows

2. HCur - ?

3. ChNam - Lists Channel Names

4. < > - ??

5. Zoom - Left click: zoom into the recording, Right click: zoom out of recording

6. Gain - Left click: increases gain, Right click: decreases gain

7. Offset - Left click: increases offset from baseline, Right click: decreases offset from baseline