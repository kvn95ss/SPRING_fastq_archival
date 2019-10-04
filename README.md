# SPRING_fastq_archival

STRONGLY RECOMMEND INSTALLING SPRING FROM - https://github.com/shubhamchandak94/Spring and importantly, export the PATH where spring is installed using the following command -

  export PATH=$PATH:/path/to/spring
  Even better if you add it to your ~/.bashrc 

SPRING is a utility which compresses fastq files. The bash script here recursively searches for fastq.gz files and compresses it to .spring file. Upon successful comrpession, the fastq.gz files are deleted. Decompression script, which is to be ran at directory containing the spring file, extracts the fastq files back if required.

The compression on default parameters are pretty good, especially for paired end fastq files. Expect at least 50% reduction in file size, essentially store two fastq files at the space of one!
.
This tool is great for archival, reducing the storage requirements hence enabling efficient storage of files.

The current script is optimized for paired data, I'll make another script for single fastq file sometime soon.
