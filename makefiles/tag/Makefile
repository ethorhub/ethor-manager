null :=
space := ${null} ${null}
TAG := -
MAKE_TAGS = --no-print-directory
%:
	$(eval _subst := $(subst $(TAG), , $@))
	$(eval _firstword := $(firstword $(_subst)))
	$(eval _filter-out := $(filter-out $(_firstword),$(_subst)))
	cd $(_firstword) && $(MAKE) $(MAKE_TAGS) $(subst $(space),$(TAG),$(_filter-out))