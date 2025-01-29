Mtb RNAseq data analysis from scratch
### Downloading the data from NCBI using SRA toolkit ####

C:\sratoolkit\bin>prefetch SRR10681572 SRR10681571 SRR10681570 SRR10681569
2025-01-28T12:52:30 prefetch.3.2.0: 1) Resolving 'SRR10681572'...
2025-01-28T12:52:33 prefetch.3.2.0: Current preference is set to retrieve SRA Normalized Format files with full base quality scores
2025-01-28T12:52:35 prefetch.3.2.0: 1) 'SRR10681572' is found locally
2025-01-28T12:52:35 prefetch.3.2.0: 1) Resolving 'SRR10681572's dependencies...
2025-01-28T12:52:35 prefetch.3.2.0: 'SRR10681572' has 0 unresolved dependencies
2025-01-28T12:52:35 prefetch.3.2.0: 2) Resolving 'SRR10681571'...
2025-01-28T12:52:37 prefetch.3.2.0: 2) Downloading 'SRR10681571'...
2025-01-28T12:52:37 prefetch.3.2.0:  SRA Normalized Format file is being retrieved
2025-01-28T12:52:37 prefetch.3.2.0:  Downloading via HTTPS...
2025-01-28T13:00:33 prefetch.3.2.0:  HTTPS download succeed
2025-01-28T13:00:33 prefetch.3.2.0:   verifying 'SRR10681571'...
2025-01-28T13:00:52 prefetch.3.2.0:  'SRR10681571' is valid: 3892984883 bytes were streamed from 3892972087
2025-01-28T13:00:52 prefetch.3.2.0: 2) 'SRR10681571' was downloaded successfully
2025-01-28T13:00:52 prefetch.3.2.0: 3) Resolving 'SRR10681570'...
2025-01-28T13:00:56 prefetch.3.2.0: 3) Downloading 'SRR10681570'...
2025-01-28T13:00:56 prefetch.3.2.0:  SRA Normalized Format file is being retrieved
2025-01-28T13:00:56 prefetch.3.2.0:  Downloading via HTTPS...
2025-01-28T13:06:54 prefetch.3.2.0:  HTTPS download succeed
2025-01-28T13:06:54 prefetch.3.2.0:   verifying 'SRR10681570'...
2025-01-28T13:07:01 prefetch.3.2.0:  'SRR10681570' is valid: 2532721730 bytes were streamed from 2532721207
2025-01-28T13:07:01 prefetch.3.2.0: 3) 'SRR10681570' was downloaded successfully
2025-01-28T13:07:01 prefetch.3.2.0: 3) Resolving 'SRR10681570's dependencies...
2025-01-28T13:07:02 prefetch.3.2.0: 'SRR10681570' has 0 unresolved dependencies
2025-01-28T13:07:02 prefetch.3.2.0: 4) Resolving 'SRR10681569'...
2025-01-28T13:07:05 prefetch.3.2.0: 4) Downloading 'SRR10681569'...
2025-01-28T13:07:05 prefetch.3.2.0:  SRA Normalized Format file is being retrieved
2025-01-28T13:07:05 prefetch.3.2.0:  Downloading via HTTPS...
2025-01-28T13:14:42 prefetch.3.2.0:  HTTPS download succeed
2025-01-28T13:14:42 prefetch.3.2.0:   verifying 'SRR10681569'...
2025-01-28T13:14:50 prefetch.3.2.0:  'SRR10681569' is valid: 4000818296 bytes were streamed from 4000816663
2025-01-28T13:14:50 prefetch.3.2.0: 4) 'SRR10681569' was downloaded successfully

C:\sratoolkit\bin>fastq-dump --split-3 C:\sratoolkit\bin\tmp\sra\SRR10681569.sra
Read 38684242 spots for /C/sratoolkit/bin/tmp/sra/SRR10681569.sra
Written 38684242 spots for /C/sratoolkit/bin/tmp/sra/SRR10681569.sra

C:\sratoolkit\bin>fastq-dump --split-3 C:\sratoolkit\bin\tmp\sra\SRR10681570.sra
Read 32515770 spots for /C/sratoolkit/bin/tmp/sra/SRR10681570.sra
Written 32515770 spots for /C/sratoolkit/bin/tmp/sra/SRR10681570.sra

C:\sratoolkit\bin>
C:\sratoolkit\bin>fastq-dump --split-3 C:\sratoolkit\bin\tmp\sra\SRR10681571.sra
Read 37637148 spots for /C/sratoolkit/bin/tmp/sra/SRR10681571.sra
Written 37637148 spots for /C/sratoolkit/bin/tmp/sra/SRR10681571.sra

C:\sratoolkit\bin>fastq-dump --split-3 C:\sratoolkit\bin\tmp\sra\SRR10681572.sra
Read 23704109 spots for /C/sratoolkit/bin/tmp/sra/SRR10681572.sra
Written 23704109 spots for /C/sratoolkit/bin/tmp/sra/SRR10681572.sra

