#This README file will describe the analytical methods used to tackle the biological question. 

The project aims to plot a PCA on isoform transcript expression in three samples across five specific brain regions. This will require me to first annotate any novel exons/novel transcripts from long-read Nanopore data through mapping it to the human transcriptome and metagene. 
## Software Dependencies 
You can clone the bioinformatics pipeline repo used to annotate and quantify the transcripts (https://github.com/twrzes/TAQLoRe ). 
Once in the repo, cd into TAQLoRe/docs/installation.rst

Follow the directions for either automated or manual software installation. 

To facilitate automated installation, use conda package manager. (https://docs.conda.io/en/latest/miniconda.html).

To facilitate manual installation of software dependencies, download each of the following: 
* Python 3.5.1)
	* pandas (0.24.2)
	* numpy (1.16.3)
	* tqdm (4.32.1)
	* pysam (0.15.2)
	* pybedtools (0.8.0)
	* scipy (1.2.1)
	* natsort (6.0.0)
	
*	Perl (5.22.1)
*	R (3.5.1)
*	Bedtools (2.26.0)
*	LAST (979)
*	GMAP (20190315)
*	Git (2.21)
*	Snakemake (5.4.5)

Once those novel isoforms are aligned and annotated, PCA will be generated through R statistical language using the following libraries: 
* pandas (0.24.2)
* numpy (1.16.3)
* tqdm (4.32.1)
* pysam (0.15.2) 
* pybedtools (0.8.0)
* scipy (1.2.1)
* natsort (6.0.0)
