SUBDIRS = foo bar baz

.PHONY: subdirs $(SUBDIRS)

subdirs: $(SUBDIRS)

$(SUBDIRS):
	$(MAKE) -C $@

foo: baz

clean:
	for dir in $(SUBDIRS); do \
		$(MAKE) clean -C $$dir; \
	done	
