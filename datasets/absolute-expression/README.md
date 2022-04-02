# Absolute Expression datasets

Absolute datasets are specific datasets that can be used to compute for each protein an absolute expression value (e.g. IBAQ). Absolute expression datasets are mainly two types of datasets DIA-LFQ and DDA-LFQ.

We have divided the datasets in four main categories:

- cell-lines: experiments from cancer cell-lines
- tissues: experiments from healthy/normal human tissues
- platelet: experiments from platelet / serum / plasma
- tumor: experiments from different tumor

Each category contains a set of folders representing the different projects annotated, in each project samples are divided as follows:

- If more than one sample are available for the same factor value (e.g. tissue, cell-line, etc) they are aggregated into one sdrf.tsv using biological or technical replicates. With this approach, we can enable in the analysis Match-Between runs for better performance o the identification results.
- If no replication is available in the project (biological or technical), the full project can be divided by samples.

## How to select datasets

For absolute expression projects, we have a set of rules to select the project to be annotated:

- Samples MUST be from healthy/normal tissues.
- For absolute quantification we will use only Trypsin-derived samples. We have decided that because, if we add more enzymes, more variability is found across experiments making difficult the final comparisons.

## Factor values

For each category the factor value is different:

- cell-lines: the factor value is the cell-line code `characteristics[cell line]`
- tissues: experiments from healthy/normal human tissues `characteristics[organism part]`
- platelet: experiments from platelet / serum / plasma `characteristics[organism part]`
- tumor: experiments from different tumor  `characteristics[disease]`

## Datasets

### Tissues

- [x] PXD000561: LFQ experiment, tissue proteomes, 2212 raw files
- [x] PXD000865: LFQ experiment, tissue proteomes, 1055 raw files
- [x] PXD010154: LFQ experiment, tissue proteomes, 1800 raw files
- [x] PXD020192: LFQ experiment, tissue proteomes, 92 raw files
- [x] PXD010271: LFQ experiment, tissue proteomes, 220 raw files
- [x] PXD004452: LFQ experiment, (colon, liver, prostate), 216 raw files

- brain:
  - [x] PXD000547 & PXD000548: LFQ experiment, brain, 80 raw files
  - [x] PXD012755: LFQ experiment, brain, 32 raw files
  - [x] PXD004143: LFQ experiment, brain, 4 raw files
  - [x] PXD005445: LFQ experiment, brain, 196 raw files (Note: Only generic samples)
  - [x] PXD006233: LFQ experiment, brain,

- skin:
  - PXD019909: LFQ experiment, skin, 152 raw files

- heart:
  - [x] PXD008934: LFQ experiment, heart, 34 raw files
  - [ ] PXD006675: LFQ experiment, heart, 594 raw files
  - [ ] PXD008722: LFQ experiment, heart, 252 raw files
  - [x] PXD018678: LFQ experiment, heart, 11 raw files
  - [ ] PXD018678: DIA-LFQ experiment, heart, 48 raw files
  - [ ] PXD012636: LFQ experiment, heart, 91 raw files
  - [ ] PXD012467: LFQ experiment, heart, (Note: needs to find the normal tissues)
  - [x] PXD011349: LFQ experiment, heart, 55 raw files
  - [ ] PXD008852: DIA-LFQ experiment, heart,
  - [x] PXD005736: LFQ experiment, heart, 24 RAW files

- stomach:
  - [ ] PXD008840: LFQ experiment, stomach, 504 raw files

- lung:
  - [x] PXD004700: LFQ experiment, lung, 46 raw files
  - [x] PXD004682: LFQ experiment, lung, 96 raw files
  - [ ] PXD004684: DIA-LFQ experiment, lung, 8 raw files

- anterior pituitary gland
  - [x] PXD005819: LFQ experiment, anterior pituitary gland, 32 raw files (Note: Sample 2 removed few peptides)

- colon mucosa
  - [x] PXD001608: LFQ experiment, colonic mucosa, 30 raw files

- ovary
  - [ ] PXD008183: Error quant in MS1.
  - [x] PXD025864 LFQ experiment, ovary, 9 raw files

- Choroid
  - [ ] PXD002273

- pancreas
  - [ ] https://www.iprox.org/page/project.html?id=IPX0001745000

- Eccrine sweat glands
  - [ ] PXD010637

- sclera
  - [ ] PXD022661
  - [x] PXD008999

- testis
  - [ ] PXD009737
  - [x] PXD002179

- kidney
  - [x] PXD006482

- Spermatozoon
  - [ ] PXD003947

- Liver
  - [ ] PXD009021

### Plasma

- [ ] PXD011839
- [ ] PXD004242

### Tumor datasets

- [ ] PXD012431

### Cell lines

### Some experiments to be seen:

- PXD018301
- PXD019643 HLA atlas
- PXD005629: A proteomic analysis of human olfactory bulb
- PXD003539: Cell lines NCI-60 DIA
- PXD020481
- PXD008032: Cancer datasets different regions
- PXD016662
- PXD005479: NCI-60
- PXD024111
- PXD006921
- PXD002775
- PXD010142: Cell lines
- PXD015087
- PXD004465

