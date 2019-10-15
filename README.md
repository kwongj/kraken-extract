# kraken-extract
Extract sequences classified as specified taxa 

# Author
Jason Kwong (@kwongjc) :: [https://github.com/kwongj](kwongj)

# Requirements
* Kraken output file
* File with list of taxa IDs
* `pigz`: optional for post extraction gzip compression of reads

# Usage
```
$ kraken-extract.py -h
usage: 
  kraken-extract.py --kraken [kraken.out] --taxids [file] READS > extracted.fastq
  kraken-extract.py --kraken [kraken.out] --taxids [file] READS | pigz > extracted.fastq.gz

extracts specified taxa sequences from Kraken classification - script by JK

positional arguments:
  READS          single FASTQ file

optional arguments:
  -h, --help     show this help message and exit
  --kraken FILE  output file from Kraken
  --taxids FILE  file with list of taxa ID to extract
  --version      show program's version number and exit
```

# Bugs
Please submit via the GitHub issues page: https://github.com/kwongj/kraken-extract/issues

# Licence
https://github.com/kwongj/kraken-extract/blob/master/LICENSE
