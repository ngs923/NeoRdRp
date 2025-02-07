## Creating RdRp HMM profiles by yourself

You can create your original RdRp HMM profiles by runnning the following script:

`python3 pipeline.py -i INPUT.FASTA`

## Recuirements
- CD-HIT
- MAFFT
- Divvier
- HMMER
- Pandas
- Biopython

## Changing parameters

Open pipeline.py and change the parameters in the parameter section: you can change CD-HIT identity (default 0.6), wordsize (default 4), and minimum sequences in the cluster (default 3).

```
# parameter
param_cdhit_threshould = str(0.6)
param_cdhit_wordsize = str(4)
param_cdhit_cluster = str(3)
```

If you need to change the definition of boundary, open cutgap.py and change the parameter: you can change threshold (default 0.25) and minimum length (default 9).

```
threshold=0.25
minlength = 9
```
