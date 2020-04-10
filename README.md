# Dependencies
* https://github.com/mozilla/pdf.js

# Installation
* `git clone https://github.com/mozilla/pdf.js`
* `mkdir pdf.js.test`
* `cp -r pdf.js/{external,src,web} pdf.js.test/`
* `cd pdf.js.test`
* `npm install`

# Troubleshooting
If you failed to render PDF in browser and got some error message from javascript console, you should execute commands as follows.
* `cp pdf.js/package.json pdf.js.test/package.json`
* `cd pdf.js.test`
* `npm install`

# Settings for locale
* `cp -r pdf.js/l10n pdf.js.test/web/locale`
* `cd pdf.js.test`
* `(echo "[ko]"; echo "@import url(ko/viewer.properties)") > web/locale/locale.properties`

# PDF file location
* You should download a pdf file and save it to the 'pdf.js.test' directory.

# Clean-up
* `rm -rf pdf.js/`

# Demo
* [https://terzeron.com/pdf.js.test/web/viewer.html?filename=jit_type.pdf](https://terzeron.com/pdf.js.test/web/viewer.html?filename=jit_type.pdf)
