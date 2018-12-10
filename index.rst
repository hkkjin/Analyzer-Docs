.. Spike Cluster Analyzer documentation master file, created by
   sphinx-quickstart on Fri Dec  7 18:08:58 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Spike Cluster Analyzer's Documentation!
==================================================

The Spike Cluster Analyzer
--------------------------

Overview
^^^^^^^^

The Spike Cluster Analyzer, first developed in TG's thesis and improved upon based on multiple projects ongoing in IS's lab, is a Matlab-based program that is made to analyze EEG data to identify spike clusters in samples obtained, for example, through the analyzer downloadable_ in CA and EKM's study, "Closed-Loop Optogenetic Intervention in Mice" (*Nature Protocols*, 2013). 

.. _downloadable: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3988315/

At the time this study was done, all seizure analysis was done manually and only very general information was annotated, such as seizure start and end. The goal is to achieve EEG data analysis that not only includes seizure/cluster length but also finer spike analysis in a semi-automated and eventually a fully automated manner.

This document is in its very early stages and will be updated as more features of this program are tested.

..

Main Features
^^^^^^^^^^^^^

Among many other functions, the Spike Cluster Analyzer is able to:

1. Perform in-depth reanalysis of data previously collected through the executable EEG analyzer `(2013 version)`_
2. Perform analysis of new EEG data
3. Perform analysis of individual spikes and clusters
4. Cross analyze results from different subjects
5. Output data to other programs 

.. _(2013 version): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3988315/


Introduction
------------

.. toctree::
   :maxdepth: 2
   :titlesonly:

   Background
   Related Studies
   

Instruction Manual
------------------

.. toctree::
   :maxdepth: 2
     
   Getting Started
   Initial Analysis
   Secondary Analysis
   Cross Analysis
   Spike Analysis


Updates and Help
----------------

.. toctree::
   :maxdepth: 2
   :titlesonly:

   Troubleshooting     
   Known Issues
   Version History


Acknowledgements
----------------

Thanks to TG and MO for creating and working a ton on this program. CV and MO worked on the earliest versions of the spike analyzer which is now a feature in TG's program. HK is currently writing this document and learning a lot about rst files.


Questions? Bug TG_, he's the expert :) I just write things. J/k, please feel free to contact me `(HK)`_ with user questions as well.

Please send suggestions for additions and edits for this manual to HK_ as well, it would be greatly appreciated!




.. _TG: gschwind@stanford.edu
.. _(HK): hkim346@stanford.edu
.. _HK: hkim346@stanford.edu



