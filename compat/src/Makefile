VERSION= 5.1
PKG= compat-$(VERSION)
DIST_DIR= $(PKG)
TAR_FILE= $(PKG).tar.gz
ZIP_FILE= $(PKG).zip
SRCS= Makefile \
	$(PKG).lua $(PKG).c $(PKG).h \
	index.html license.html compat.png

dist: dist_dir
	tar -czf $(TAR_FILE) $(DIST_DIR)
	zip -lq $(ZIP_FILE) $(DIST_DIR)/*
	rm -rf $(DIST_DIR)

clean:
	rm $(TAR_FILE) $(ZIP_FILE)

dist_dir:
	mkdir -p $(DIST_DIR)
	cp $(SRCS) $(DIST_DIR)
