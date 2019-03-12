# GERMSLab Wafergen SOP

## Before Run

1. Create a file of metadata for your samples.  It should contain a unique sample identifier and associated metadata for each sample.  An example is shown below.

[Jin can you put an example here]

2. Create a file of the primers used, and name it primers_yourname_date (e.g., primers_howe_190318) for Adina Howe's primers used on March 18, 2019.

[Jin can you put an example here]

3. Design your plate layout. Name this file layout_yourname_date. [Lanying can you put instructions here as needed]

4. Make a folder in the Box Drive Folder - GERMS-Wafergen [https://iastate.box.com/s/g0tt6382aagmd3eut4at2bgljhipi53g] to place the three files above in.  Name that folder as wafergen_yourname_date.



## After run

1.  Place the raw data downloaded from MSU into the folder you created above.  Rename that file rawdata_yourname_date_of_the_run.

2.  [Jin please put documentation on how to process data with an output of something I can use to keep track of standard curves]

You will have txt file after data back from MSU. Use Rscript_for_wafergen.R for analyzing data. You will need 1) txt formatted data file 2) meta data for samples 3) meta for standard. Then use R to run

3.  Place your standard curve data in the spreadsheet located in the Box Drive Folder - GERMS-Wafergen --> Standard_Curves
