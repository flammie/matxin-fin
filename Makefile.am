RELEASE=0.0
VERSION=0.0.0
LANG1=fin
BASENAME=matxin-$(LANG1)


TARGETS_COMMON=$(LANG1).deprlx.bin

$(LANG1).deprlx.bin: $(BASENAME).$(LANG1).deprlx $(CGCOMP)
	$(CGCOMP) $< $@

## Distribution

EXTRA_DIST=$(BASENAME).$(LANG1).deprlx

## Installation

matxin_findir=$(prefix)/share/matxin/$(BASENAME)/
matxin_fin_srcdir=$(prefix)/share/matxin/$(BASENAME)/

matxin_fin_DATA=$(TARGETS_COMMON)

pkgconfigdir = $(prefix)/share/pkgconfig
pkgconfig_DATA = $(BASENAME).pc

CLEANFILES = $(TARGETS_COMMON)
clean-local:
	-rm -rf .deps modes

## Tests
