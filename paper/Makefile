chaucer-macro-etym.pdf: chaucer-macro-etym.md
	pandoc -o $@ $< \
		--latex-engine=xelatex \
		-V colorlinks \
		-V mainfont='Linux Libertine O' \
		--filter pandoc-crossref \
		--filter pandoc-citeproc
	evince $@ &

chaucer-macro-etym.docx: chaucer-macro-etym.md
	pandoc -o chaucer-macro-etym.docx $< \
		-V colorlinks \
		--filter pandoc-crossref \
		--filter pandoc-citeproc
	libreoffice $@ &
