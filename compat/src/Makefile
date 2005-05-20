VERSION= r3
PKG= compat-5.1$(VERSION)
DIST_DIR= $(PKG)
TAR_FILE= $(PKG).tar.gz
ZIP_FILE= $(PKG).zip
FILES= Makefile \
	index.html license.html compat.png
SRCS= compat-5.1.lua compat-5.1.c compat-5.1.h

dist: dist_dir
	tar -czf $(TAR_FILE) $(DIST_DIR)
	zip -rq $(ZIP_FILE) $(DIST_DIR)/*
	rm -rf $(DIST_DIR)

clean:
	rm $(TAR_FILE) $(ZIP_FILE)

dist_dir:
	mkdir -p $(DIST_DIR)
	cp $(SRCS) $(DIST_DIR)

	