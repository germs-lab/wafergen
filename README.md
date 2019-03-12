# Python code for generating CSV file for robot
For SOP, please see here https://github.com/germs-lab/SOPs/blob/master/Wafergen.md

## If you use Bob's primer use command like this
```
python prepare_bob_primer_144S_36A.py lan_list_target.txt bob_primer_plate.clean.tsv
```

## This is made for Nitrogen cycle gene
```
python python wafergen/prepare_primer_96S_54A.py 54assays_primer_list.csv full_primer_location.csv 
```

## After run, you can use this R code to generate count
https://github.com/germs-lab/wafergen/blob/master/Rscript_for_wafergen.R

To Run,
1. Open R

2. Change path

3. Run R



