## How to prepare primer (Assay) plate for wafergen
Written by Lanying Ma, edited by Jin Choi
## Background:
This SOP is trying to walk you through how to prepare primer plate with Robot for Wafergen run.  As we have 8 plates of Bob primers about antibiotic resistant genes (384 primers with F and R primers), it would be too easy to make mistakes manually preparing the primer plates.  Thus, we try to automate it by Robot.  All the python codes were written by Jin in this SOP.  If you have any questions on it, please talk to him.  All files needed in this SOP were in germs-lab github. https://github.com/germs-lab/wafergen
## Procedures:
* 1 The first file needed is bob_primer_plate.clean.tsv. In this file, there are information on the primer position: in which plate, in which well, and sequencing Name F or R.
* 2 Make a list of your targeted primers: list_target.txt. 
   * This list will simply have the primers names which should be the same as the names in bob_primer_plate.clean.tsv.
* 3 run Python: python prepare_bob_primer.py list_target.txt bob_primer_plate.clean.tsv
   * this code will generate two files: for_Robot.tsv and for_Record.csv.  For_Robot_tsv will be the file you copy to Robot computer to tell Robot from which target plate and postion to which particular well of your primer plate.
* 4 Run Robot with for_robot.tsv to prepare the primer plate.
It will need 16 ul water with 2 ul of each F/R primers.

