Cross Analysis
--------------

Once all the desired recording files have been analyzed, the next step is to compare between groups and plot results. I haven't done this yet so this will be written once I try it out.


Plotting Results
^^^^^^^^^^^^^^^^

The **Collection** function can be used to gather results and output plots for comparison

  1. Click **Collection**

     - *coming soon*

  2. For adding a new type plot to *groups* not already available in the program




     - specify in GUI (gpoptions), specifically in init_gpoptions.m
	
	

        #. Name of the plot (pstr; line 13)
	
	

        #. Describe the plot (plotdescibstr; line 14)


     - add plotting to Step3, specifically to group_process2.m - add *plot* at the end
	
	

        #. Collect the data you need (e.g. create mean) from vrr
	
	

        #. Plot or refer to separate plot function
