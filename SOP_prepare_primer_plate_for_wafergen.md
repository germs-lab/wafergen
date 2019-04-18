## How to prepare primer (Assay) plate for wafergen by Robot
Written by Lanying Ma, edited by Jin Choi
## Background:
This SOP is trying to walk you through how to prepare primer plate with Robot for Wafergen run.  As we have 8 plates of Bob primers about antibiotic resistant genes (384 primers with F and R primers), it would be too easy to make mistakes manually preparing the primer plates.  Thus, we try to automate it by Robot. 

## Procedures:
1. The first file needed is [bob_primer_plate.clean.tsv](add @jin link).  In this file, there are information on the primer position: in which plate, in which well, and sequencing Name including F or R.
2. You should have a list of your targeted primers from the general [Wafergen SOP](https://github.com/germs-lab/SOPs/blob/master/wafergen_SOPs/wafergen-general.md) Step 3, primers_yourname_date

It is critically important that your list match primer names in file from step #1.

3. Download this [file](Jin Add this link).  Run Python: python prepare_bob_primer.py list_target.txt bob_primer_plate.clean.tsv
4. This code will generate two files: for_Robot.tsv and for_Record.csv.  For_Robot_tsv will be the file you copy to Robot computer to tell Robot from which target plate and postion to which particular well of your primer plate.
* 4 Run Robot with for_robot.tsv to prepare the primer plate.

It will need 16 ul water with 2 ul of each F/R primers.


