prokka: anno.t_rebecca/t_rebecca.txt anno.t_lynn/t_lynn.txt \
	anno.t_centrarchi/t_centrarchi.txt anno.t_maritimum/t_maritimum.txt \
	anno.t_mesophilum/t_mesophilum.txt anno.t_ovolyticum/t_ovolyitcum.txt \
	anno.t_soleae/t_soleae.txt anno.t_sp47/t_sp47.txt

t_rebecca_wt.fa/t_rebecca.txt:
	curl -L -o $@ 'https://osf.io/27cvw/?action=download'

anno.t_rebecca/t_rebecca.txt: t_rebecca_wt.fa
	prokka --outdir $@ --prefix t_rebecca $<

t_lynn_wt.fa:
	curl -L -o $@ 'https://osf.io/8c9zs/?action=download'

anno.t_lynn/t_lynn.txt: t_lynn_wt.fa
	prokka --outdir $@ --prefix t_lynn $<

t_centrarchi.fa:
	curl -L -o $@ 'https://osf.io/tney3/?action=download'

anno.t_centrarchi/t_centrarchi.txt: t_centrarchi.fa
	prokka --outdir $@ --prefix t_centrarchi $<

t_maritimum.fa:
	curl -L -o $@ 'https://osf.io/juesb/?action=download'

anno.t_maritimum/t_maritimum.txt: t_maritimumfa
	prokka --outdir $@ --prefix t_maritimum $<

t_mesophilum.fa:
	curl -L -o $@ 'https://osf.io/djwtm/?action=download'

anno.t_mesophilum/t_mesophilum.txt: t_mesophilum.fa
	prokka --outdir $@ --prefix t_mesophilum $<

t_ovolyticum.fa:
	curl -L -o $@ 'https://osf.io/xsv7c/?action=download'

anno.t_ovolyticum/t_ovolyticum.txt: t_ovolyticum.fa
	prokka --outdir $@ --prefix t_ovolyticum $<

t_soleae.fa:
	curl -L -o $@ 'https://osf.io/ub2ae/?action=download'

anno.t_soleae/t_soleae.txt: t_soleae.fa
	prokka --outdir $@ --prefix t_soleae $<

t_sp47.fa:
	curl -L -o $@ 'https://osf.io/4f3nk/?action=download'

anno.t_sp47/t_sp47.txt: t_sp47.fa
	prokka --outdir $@ --prefix t_sp47 $<
