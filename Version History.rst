Version History
---------------

`Instruction Manual Version History`_

`Analyzer Version History`_



.. _Instruction Manual Version History:

Instruction Manual Version History
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Version 1.05**

*12/11/18*

Added a glossary under the page "Spike Cluster Analyzer UI"

Added some information to "Cross Analysis"

Modified how to run the program with the new version


**Version 1.01**

*12/9/18*

Updated **Step1** under *Initial Analysis*

Reorganized information to follow a more logical progression

Minor Edits

**Version 1.00**

*12/7/18*

First version published to ReadtheDocs


.. _Analyzer Version History:

Analyzer Version History
^^^^^^^^^^^^^^^^^^^^^^^^

*(This will not be totally up to date and more based on usage than actual changes to coding)*

**Version 12/11/18**

Reorganized program into smaller number of folders

Added feature to go back during **AnalysisB**


**Version 12/7/18**

Fixed the problem where creating a credential file saved the .cre file into the GUI Settings folder


**Version 12/7/18**

Fixed the problem where during **AnalysisB** the modified thresholds for the cluster are not carried over to the next cluster.


**Version 12/6/18**

First release, this is the version that should be standardized between all new users.


The errors are currently still the same as 1.01:

1. The Step1 function gave an error when attempting to use it

2. The credential file still creates to within the Matlab folder (not good since the matlab folder with the program shouldn't be altered)


**Version 12/5/18**

Fixed: New clusters can now be added prior to the first or after the last cluster overlaid from an Excel data sheet


A few more issues:

1. The Step1 function gave an error when attempting to use it

2. The credential file still creates to within the Matlab folder (not good since the matlab folder with the program shouldn't be altered)


**Version 12/4/18**

This initial version of the SC Analyzer was used to overlay analysis output which had been cut and pasted from the original .txt output files to Excel. (to do this we used text to columns delimited by spaces)




A number of issues occurred when attempting this:



1. Analyzers prior to 2014 output cluster info differently than Analyzers used 2014 and onwards. Make sure the first column is the date and the second column is the time. Newer Analyzers include more information and these should be deleted.



2. The *Refine* function, which is used to adjust or add or delete previously marked clusters, did not work when you attempt to new clusters outside the bounds of the overlay of the previous analysis. 



3. The green markers which indicate the first detected seizure in the overlay did not always appear on the first seizure. This was due to the data in the Excel file not being in chronological order. Therefore in future tests, the first step was to make sure to sort all data by date and time prior to using *Refine*.



4. In addition, occasionally using the mouse and key combinations that should delete specific seizures did not work. Adding new seizures after this occurred caused more errors as well.



5. The **Processing** indicator kept appearing even when the processing was not taking place. Fixed by TG. 





**Version 0.1**

*A long time ago...Actually about 2016*

TG started this project during his initial visit to IS's group in 2016 when he first designed his project to analyze and intervene during interictal spikes.
