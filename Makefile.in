all:
	cd src/optipng && \
	$(MAKE) && \
	cd ../..

test:
	cd src/optipng && \
	$(MAKE) test && \
	cd ../..

check: test

install:
	cd src/optipng && \
	$(MAKE) install && \
	cd ../..

uninstall:
	cd src/optipng && \
	$(MAKE) uninstall && \
	cd ../..

clean:
	cd src/optipng && \
	$(MAKE) clean && \
	cd ../..

distclean:
	cd src/optipng && \
	$(MAKE) distclean && \
	cd ../..
	-rm -f src/Makefile Makefile

install-shared:
	cd src && \
	$(MAKE) sharedlib && \
	mkdir -p /opt/optipng/include && \
	mkdir -p /opt/optipng/lib && \
	cd .. && \
	cp -v src/liboptipng.so /opt/optipng/lib && \
	cp -v src/optipng/optipng.h src/optipng/bitset.h /opt/optipng/include
