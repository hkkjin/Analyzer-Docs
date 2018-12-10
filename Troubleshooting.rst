Troubleshooting
---------------

**For updating Spike Cluster Analyzer**

  1. If you are attempting to update the *Spike Cluster Analyzer* using Git BASH and see
   
     *error: Your local changes to the following files would be overwritten by merge:*

  2. First, make a copy of your settings files that caused this error because they will be overwritten (the names of the settings files should show up after the error message), then type in 

     ``$ git reset --hard`` 
    
     to overwrite your settings files using the default files, then continue with the update:

     ``$ git pull origin master``

  3. Replace the default settings files with the copied versions of your most recent settings.
     

**For errors while running Spike Cluster Analyzer**

At the moment the best way to solve incidental errors is to reboot the analyzer. If you have to reboot anytime after you have already created your cluster file, follow these steps:

  1. Close MATLAB Analyzer window

  .. 

  2. Run *analyzer*

  ..

  3. Once the Analyzer has launched, click on **load cluster data**

  ..

  4. Click **Open File** and open the desired MATLAB recording file

  ..

  5. Click on **ps** and other categories to view the previously saved clusters

  ..

  6. Depending on which step you were on when the error happened, you may have to run **Refine** or **AnalysisB** once again

