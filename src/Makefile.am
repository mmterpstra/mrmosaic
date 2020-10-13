bin_PROGRAMS = cnvbafdata
cnvbafdata_SOURCES = cnv_baf_data.c
cnvbafdata_CFLAGS =  -O3 -Wall -Isrc -I. -I../samtools-1.3/htslib-1.3/htslib -I../samtools-1.3/htslib-1.3 -I../samtools-1.3 -rdynamic -L../samtools-1.3.1/htslib-1.3/ -L../samtools-1.3.1/ -L../ -lhts -lpthread -lz -lm -lbam
#gcc -O3 -Wall -Isrc -I. -Ihtslib-1.3/ -Ihtslib-1.3/htslib -rdynamic -o cnv_baf_data -Lhtslib-1.3/ -L. cnv_baf_data.c -lhts -lbam -lpthread -lz -lm

