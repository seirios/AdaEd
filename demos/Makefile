TEST_RUNS := run1 \
			 run2 \
			 run3 \
			 run4 \
			 run5 \
			 run6 \
			 run7 \
			 run8 \
			 run9 \
			 runa \
			 runb \
			 rune \
			 runf \
			 rung
ALL_RUNS := $(TEST_RUNS) \
			runc \
			rund

INSTALLDIR := ../local

check: $(TEST_RUNS)

.PHONY: $(ALL_RUNS)
rung: ENVVARS := INT=..
$(ALL_RUNS): | local/
	PATH=local/bin:$$PATH $(ENVVARS) ./$@

local/:
	ln -s $(INSTALLDIR)
