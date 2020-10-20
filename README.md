# m6A_ES
All the data and source code for m6A excited states paper

### This is all the source data and code files for the m6A Excited states paper
### Ref: Liu et al, (2020) "m6A delays base-pairing through syn-anti isomerization of the methylamino group" BioRxiv

### 1. MD force field parameters (MD_forcefield)
#### m6a_new_rna.lib - force field parameters for m6A. 
#### Load using ‘loadOff m6a_new_rna.lib’ in tleap module of AMBER suite
#### DMA_rna_parmbsc0.off and DMA_rna_parmbsc0.frcmod - force field parameter files for m62A.
#### Load using ‘loadOff DMA_rna_parmbsc0.off’ and ‘loadamberparams DMA_rna_parmbsc0.frcmod’ in tleap module of AMBER suite

### 2. Input RNA duplex (dsGGACU) structures for DFT calculation (dsRNA_structure)
#### In the folder, there are five ensembles, each of ensemble contains 100 conformers. DFT is computing the average of them.
#### dsGGACU.pdb: unmodified duplex
#### dsGGACUm6Aanti.pdb: m6A modified dsGGACU at residue 6, the m6A N6-methylamino group is in anti conformation
#### dsGGACUm6Asyn.pdb: m6A modified dsGGACU at residue 6, the m6A N6-methylamino group is in syn conformation
#### dsGGACUm6Aantistar.pdb: m6A modified dsGGACU at residue 6, the m6A N6-methylamino group is in anti* conformation
#### dsGGACUm62A.pdb: m62A modified dsGGACU at residue 6


### 3. Input mononucleoside structures for DFT calculation (mono_structure)
#### In the folder, there are three subfolders representing three different mononucleoside structures.
#### "rA" is the unmodified adenosine
#### "m62rA" is the m62A modified adenosine
#### "m6rA" is the m6A modifition, where the N6-methylamino group is rotated from 0 to 360 degree


#### HO2' means the hydroxl proton connect to O2'
#### HO3' means the hydroxl proton connect to O3'
#### HO5' means the hydroxl proton connect to O5'
#### 
#### C10 means the N6-methylamino group carbon in m6A
#### H20 H21 H22 means the N6-methyl group proton in m6A
#### 
#### C11 means the second N6-methylamino group carbon in m62A
#### H23 H24 H25 means the second N6-methyl group proton in m62A
#### 
#### OP3 means the fourth oxygen in phosphate acid group in monophosphate structure
#### 
#### monophosphate has two negative charge
#### 
#### m6A is named as M6A
#### m62A is named as DMA


