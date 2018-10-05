# ![NGI-RNAfusion](https://raw.githubusercontent.com/SciLifeLab/NGI-RNAfusion/master/docs/images/NGI-RNAfusion_logo.png)


# This pipeline has moved!

This pipeline has been moved to the new [nf-core](http://nf-co.re/) project.
You can now find it here:

### https://github.com/nf-core/rnafusion

If you have any problems with the pipeline, please create an issue at the above repository instead.

To find out more about nf-core, visit [http://nf-co.re/](http://nf-co.re/)

This repository will be archived to maintain the released versions for future reruns, in the spirit of full reproducibility.

If you have any questions, please get in touch: support@ngisweden.se

// [Phil Ewels](http://github.com/ewels/), 2018-10-05

---



## *NB* This is work in progress - use at your own risk!

Attempt at setting up a pipeline for fusion detection as an addon to the previously existing NGI-RNAseq pipeline.

## Usage:
### ` --reads`
Path to input reads
**NB: Must be enclosed in quotes!**
```
 --reads 'path/to/data/sample_*_{1,2}.fastq'
```

### `--star-fusion`
If this flag is set to true then the pipeline will run STAR-Fusion.
True by default

### `--fusioncatcher`

If this flag is set to true then the pipeline will run Fusion Catcher.
True by default

More than one of these can be true at a time.

Example usage if you wish to run both STAR-fusion and Fusion Catcher
```
nextflow run /NGI-RNAfusion/main.nf --star --fusioncatcher --reads 'SRR5665649_{1,2}*.gz'
```

### `--fc_extra_options`

Invoking this flag allows for extra options to be sent directly to Fusion Catcher.

---

[![SciLifeLab](https://raw.githubusercontent.com/SciLifeLab/NGI-RNAfusion/master/docs/images/SciLifeLab_logo.png)](http://www.scilifelab.se/)
[![National Genomics Infrastructure](https://raw.githubusercontent.com/SciLifeLab/NGI-RNAfusion/master/docs/images/NGI_logo.png)](https://ngisweden.scilifelab.se/)

---
