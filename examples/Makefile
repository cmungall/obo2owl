%-exp.owl: %.owl
	thea-owl-i  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owl > $@

%-exp.owlpl: %.owl
	thea-owl-i  --ensure_loaded owlmacros/owlmacros $< --debug owlmacros --goal expand_all --to owlpl > $@

%.owl: %.obo
	go2owl $< > $@
