VERSION= 5.1
PKG= compat-$(VERSION)
TAR_FILE= $(PKG).tar.gz
ZIP_FILE= $(PKG).zip
SRCS= Makefile \
	$(PKG).lua $(PKG).c $(PKG).h \
	index.html license.html

dist:
	mkdir $(PKG)
	cp $(SRCS) $(PKG)
	tar -czf $(TAR_FILE) $(PKG)
	zip -lq $(ZIP_FILE) $(PKG)/*
	rm -rf $(PKG)

clean:
	rm $(TAR_FILE) $(ZIP_FILE)
