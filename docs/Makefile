---
---
PATH := ../node_modules/.bin:$(PATH)

FA_ROOT_DIRECTORY = assets/font-awesome

SITE_LESS_DIRECTORY = assets/less
SITE_CSS_DIRECTORY = assets/css

SITE_LESS = ${SITE_LESS_DIRECTORY}/site.less
SITE_CSS = ${SITE_CSS_DIRECTORY}/site.css

build:
	@echo "Compiling Less files"

	bundle exec lessc --compress ${SITE_LESS} > ${SITE_CSS}

	find .. -type f ! -perm 644 -exec chmod 644 {} \;

default: build


.PHONY: build
