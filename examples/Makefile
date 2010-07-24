# Thea is required for macro-expansion
#  See http://github.com/vangelis/thea/
%-exp.owl: %.owl
	thea  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owl > $@

%-exp.owlpl: %.owl
	thea  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owlpl > $@

# go-perl is required for obo->owl conversion
# (note currently requires latest version from cvs)
%.owl: %.obo
	go2owl $< > $@
