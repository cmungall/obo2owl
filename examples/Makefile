# Thea is required for macro-expansion
#  See http://github.com/vangelis/thea/
%-exp.owl: %.owl
	thea  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owl > $@

%-exp.owlpl: %.owl
	thea  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owlpl > $@

# see oboformat project on googlecode
%.owl: %.obo
	obolib-obo2owl $< -o file://`pwd`/$@
#go2owl $< > $@
