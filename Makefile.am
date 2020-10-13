SUBDIRS = src scripts
dist_doc_DATA = README

install-r:
	Rscript -e 'install.packages("mrmosaic", repos=NULL, type="source")'
clean-local:
	@rm config.status configure config.log
	@rm Makefile
	@rm -r autom4te.cache/
	@rm aclocal.m4
	@rm compile install-sh missing Makefile.in
