all:
	cd optipng && \
	$(MAKE) && \
	cd ..

test:
	cd optipng && \
	$(MAKE) test && \
	cd ..

check: test

install:
	cd optipng && \
	$(MAKE) install && \
	cd ..

uninstall:
	cd optipng && \
	$(MAKE) uninstall && \
	cd ..

clean:
	cd optipng && \
	$(MAKE) clean && \
	cd ..

distclean:
	cd optipng && \
	$(MAKE) distclean && \
	cd ..
	-rm -f ../Makefile Makefile

sharedlib: all
	gcc -shared -o liboptipng.so optipng/optim.o optipng/bitset.o optipng/ioutil.o optipng/ratio.o optipng/wildargs.o pngxtern/libpngxtern.a opngreduc/libopngreduc.a zlib/libz.a gifread/libgifread.a pnmio/libpnmio.a minitiff/libminitiff.a -lm