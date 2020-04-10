# Dependencies
* https://github.com/mozilla/pdf.js

# Installation
* `git clone https://github.com/mozilla/pdf.js`
* `mkdir pdf.js.test`
* `cp -r pdf.js/{external,src,web} pdf.js.test/`
* `cd pdf.js.test`
* `npm install --save requirejs`

# Locale
* `(echo "[ko]"; echo "@import url(ko/viewer.properties)") > web/locale/locale.properties`
* `cp -r pdf.js/i10n pdf.js.test/web/locale`

# Clean-up
* `rm -rf pdf.js`

# Demo
* [https://terzeron.com/pdf.js.test](https://terzeron.com/pdf.js.test)
