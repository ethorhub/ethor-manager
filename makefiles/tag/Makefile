null :=
space := ${null} ${null}
TAG := -_-
MAKE_TAGS = --no-print-directory
%:
	$(eval _subst := $(subst $(TAG), , $@))
	$(eval _firstword := $(firstword $(_subst)))
	$(eval _filter-out := $(filter-out $(_firstword),$(_subst)))
	@echo "\e[7m ETHOR(tag) \033[92m cd $(_firstword) && $(MAKE) $(MAKE_TAGS) $(subst $(space),$(TAG),$(_filter-out)) \033[0m"
	@cd $(_firstword) && $(MAKE) $(MAKE_TAGS) $(subst $(space),$(TAG),$(_filter-out))