# Dependencies
* https://github.com/mozilla/pdf.js

# Installation
# Short version
* `git clone https://github.com/terzeron/PDFjsTest pdf.js.test`
* `cp -r pdf.js/{external,src,web} pdf.js.test/`
* `cd pdf.js.test`
* `npm install`

# Long version
# copy some files from mozilla/pdf.js
* `git clone https://github.com/mozilla/pdf.js`
* `mkdir pdf.js.test`
* `cp -r pdf.js/{external,src,web} pdf.js.test/`
* `cd pdf.js.test`
* `npm install --save requirejs`
* `npm install --save core-js@3.6.4`
* `npm install --save systemjs@0.21.6`
* `npm install --save systemjs-plugin-babel@0.0.25`
* `npm install --save web-streams-polyfill@2.1.0`

# settings for locale
* `cp -r pdf.js/l10n pdf.js.test/web/locale`
* `cd pdf.js.test`
* `(echo "[ko]"; echo "@import url(ko/viewer.properties)") > web/locale/locale.properties`

# Troubleshooting
If you failed to render PDF in browser and got some error message from javascript console, you should execute commands as follows.
* `cp pdf.js/package.json pdf.js.test/package.json`
* `cd pdf.js.test`
* `npm install`

# PDF file location
* You should download a pdf file and save it to the 'pdf.js.test' directory.

# Clean-up
* `rm -rf pdf.js/`

# Demo
* [https://terzeron.com/pdf.js.test/web/viewer.html?filename=jit_type.pdf](https://terzeron.com/pdf.js.test/web/viewer.html?filename=jit_type.pdf)
