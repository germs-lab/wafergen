# Prepare primer plate for wafergen using Bob's primer and/or Nitrogen primer
This repository contains python code for preparing primer plate using bob's primer or Nitrogen primers. The python codes in the repository helps you to create CSV files for robot. If you are looking for a general SOP for preparing wafergen, please see here https://github.com/germs-lab/SOPs/blob/master/wafergen_SOPs/wafergen-general.md

### If you use Bob's primer use command like this
```
python prepare_bob_primer_144S_36A.py lan_list_target.txt bob_primer_plate.clean.tsv
```

### This is made for Nitrogen cycle gene
```
python prepare_primer_96S_54A.py 54assays_primer_list.csv full_primer_location.csv 
```

# For analzing qPCR data
## This detailed tutorial shows how to anlaze qPCR data using R
http://germslab.org/wafergen/wafergenR.html


