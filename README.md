# Dynamic Activities


## Known issues

If you need to create new icon files, `fontcustom compile` doesn't work locally.

1. https://gitpod.io/#https://github.com/davidjon/fontcustom.git and follow the installation instructions on git
2. https://github.com/FontCustom/fontcustom#installation
  - `brew tap bramstein/webfonttools && brew install woff2 && brew install fontforge && brew install eot-utils && gem install fontcustom`

3. The compiling won't complete due to non-executable `sfnt2woff`.
4. Manually, add the icons to the array in `font-icons.scss`.
5. Push changes, and pull them locally.
6. Go to https://convertio.co/nl/ttf-woff/ and convert the current `.ttf` file to woff.
7. Afterwards run `base64 icons.woff > icons.ttf` and copy and paste in `icon-font.scss`

Then every works.
