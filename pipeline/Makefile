all: prokka quast

prokka: anno.t_rebecca/t_rebecca.txt anno.t_lynn/t_lynn.txt \
	anno.t_centrarchi/t_centrarchi.txt anno.t_maritimum/t_maritimum.txt \
	anno.t_mesophilum/t_mesophilum.txt anno.t_ovolyticum/t_ovolyticum.txt \
	anno.t_soleae/t_soleae.txt anno.t_sp47/t_sp47.txt

quast: quast.t_rebecca/report.txt quast.t_lynn/report.txt quast.t_centrarchi/report.txt quast.t_maritimum/report.txt quast.t_mesophilum/report.txt quast.t_ovolyticum/report.txt quast.t_soleae/report.txt

t_rebecca_wt.fa:
	curl -L -o $@ 'https://osf.io/27cvw/?action=download'

anno.t_rebecca/t_rebecca.txt: t_rebecca_wt.fa
	prokka --outdir $(dirname $@) --prefix t_rebecca $<

quast.t_rebecca/report.txt: t_rebecca_wt.fa
	quast.py -o quast.t_rebecca $<

t_lynn_wt.fa:
	curl -L -o $@ 'https://osf.io/8c9zs/?action=download'

anno.t_lynn/t_lynn.txt: t_lynn_wt.fa
	prokka --outdir $(dirname $@) --prefix t_lynn $<

quast.t_lynn/report.txt: t_lynn_wt.fa
	quast.py -o quast.t_lynn $<

t_centrarchi.fa:
	curl -L -o $@ 'https://osf.io/tney3/?action=download'

anno.t_centrarchi/t_centrarchi.txt: t_centrarchi.fa
	prokka --outdir $(dirname $@) --prefix t_centrarchi $<

quast.t_centrarchi/report.txt: t_centrarchi.fa
	quast.py -o quast.t_centrarchi $<

t_maritimum.fa:
	curl -L -o $@ 'https://osf.io/juesb/?action=download'

anno.t_maritimum/t_maritimum.txt: t_maritimum.fa
	prokka --outdir $(dirname $@) --prefix t_maritimum $<

quast.t_maritimum/report.txt: t_maritimum.fa
	quast.py -o quast.t_maritimum $<

t_mesophilum.fa:
	curl -L -o $@ 'https://osf.io/djwtm/?action=download'

anno.t_mesophilum/t_mesophilum.txt: t_mesophilum.fa
	prokka --outdir $(dirname $@) --prefix t_mesophilum $<

quast.t_mesophilum/report.txt: t_mesophilum.fa
	quast.py -o quast.t_mesophilum $<

t_ovolyticum.fa:
	curl -L -o $@ 'https://osf.io/xsv7c/?action=download'

anno.t_ovolyticum/t_ovolyticum.txt: t_ovolyticum.fa
	prokka --outdir $(dirname $@) --prefix t_ovolyticum $<

quast.t_ovolyticum/report.txt: t_ovolyticum.fa
	quast.py -o quast.t_ovolyticum $<

t_soleae.fa:
	curl -L -o $@ 'https://osf.io/ub2ae/?action=download'

anno.t_soleae/t_soleae.txt: t_soleae.fa
	prokka --outdir $(dirname $@) --prefix t_soleae $<

quast.t_soleae/report.txt: t_soleae.fa
	quast.py -o quast.t_soleae $<

t_sp47.fa:
	curl -L -o $@ 'https://osf.io/4f3nk/?action=download'

anno.t_sp47/t_sp47.txt: t_sp47.fa
	prokka --outdir $(dirname $@) --prefix t_sp47 $<
